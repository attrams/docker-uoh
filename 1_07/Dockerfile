# Set image to ubuntu 24.04
FROM ubuntu:24.04

# Use /usr/src/app as our workdir.
WORKDIR /usr/src/app

# Copy the script.sh file from this directory to /usr/src/app
COPY script.sh .

# Make the script executable
RUN chmod +x script.sh

# Install curl
RUN apt-get update && apt-get install -y curl && rm -r /var/lib/apt/lists/*

# When running docker run the command will be ./script.sh
CMD ["./script.sh"]
