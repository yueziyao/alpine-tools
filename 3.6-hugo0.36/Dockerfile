FROM alpine:3.7

ENV HUGO_VERSION 0.36
ENV HUGO_BINARY hugo_${HUGO_VERSION}_Linux-64bit

# Install pygments (for syntax highlighting)
RUN apk add --no-cache py-pygments git bash 

ADD https://github.com/spf13/hugo/releases/download/v${HUGO_VERSION}/${HUGO_BINARY}.tar.gz /usr/local/
RUN tar xzf /usr/local/${HUGO_BINARY}.tar.gz -C /usr/local/bin/ \
	&& rm /usr/local/${HUGO_BINARY}.tar.gz

