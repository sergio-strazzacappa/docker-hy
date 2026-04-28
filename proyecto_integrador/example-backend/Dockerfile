FROM debian:trixie-slim

RUN apt-get update && apt-get -y install \
    curl \
    tar

WORKDIR /usr/src/app

ENV GO_VERSION=26.1
RUN curl -fsSL https://go.dev/dl/go1.${GO_VERSION}.linux-amd64.tar.gz | tar -C /usr/local -xzf -

ENV PATH="/usr/local/go/bin:${PATH}"
COPY . .

RUN useradd -m appuser

RUN go build

USER appuser
ENV REQUEST_ORIGIN=http://localhost:8000
ENV PORT=8080
EXPOSE 8080
CMD ["./server"]
