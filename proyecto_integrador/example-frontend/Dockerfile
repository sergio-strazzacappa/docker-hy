FROM ubuntu:latest

# Install necessary packages
RUN apt-get update && apt-get -y install curl

# Install nodejs
RUN curl -sL https://deb.nodesource.com/setup_16.x | bash
RUN apt install -y nodejs

WORKDIR /usr/src/app

# Install dependencies
COPY package* .
RUN npm install

# Build the aplication
COPY . .
ENV REACT_APP_BACKEND_UR=/api
RUN npm run build
RUN npm install -g serve

RUN useradd -m appuser
USER appuser

# Run the aplication
EXPOSE 5001
CMD ["serve", "-s", "-l", "5001", "build"]
