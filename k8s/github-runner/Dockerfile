FROM myoung34/github-runner:latest

# The base image ships curl 7.68 (Ubuntu 20.04) with OpenSSL 1.1.1.
# Cloudflare blocks this old TLS fingerprint. Replace with a static
# curl build that uses a modern TLS stack.
RUN curl -fsSL https://github.com/moparisthebest/static-curl/releases/latest/download/curl-amd64 \
      -o /usr/local/bin/curl && \
    chmod +x /usr/local/bin/curl
