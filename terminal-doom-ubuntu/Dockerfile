FROM ubuntu:latest

# Update the base system and install necessary packages
RUN apt-get update && apt-get upgrade -y \
    && apt-get install -y git build-essential curl jq 
    
# Start of Selection
RUN curl -L https://ziglang.org/download/0.13.0/zig-linux-x86_64-0.13.0.tar.xz -o zig.tar.xz \
    && tar -xJf zig.tar.xz -C /usr/local/bin --strip-components=1 \
    && rm zig.tar.xz

WORKDIR /app

RUN git clone --depth 1 https://github.com/cryptocode/terminal-doom.git terminal-doom 

WORKDIR /app/terminal-doom 

RUN zig build -Doptimize=ReleaseFast

CMD ["zig-out/bin/terminal-doom"]
