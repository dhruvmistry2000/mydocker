FROM alpine:latest

RUN apk add --no-cache git build-base curl jq \
    && curl -L https://ziglang.org/download/0.13.0/zig-linux-x86_64-0.13.0.tar.xz -o zig.tar.xz \
    && tar -xJf zig.tar.xz -C /usr/local/bin --strip-components=1 \
    && rm zig.tar.xz

WORKDIR /app

RUN git clone --depth 1 https://github.com/cryptocode/terminal-doom.git

WORKDIR /app/terminal-doom

RUN zig build -Doptimize=ReleaseFast

CMD ["zig-out/bin/terminal-doom"]
