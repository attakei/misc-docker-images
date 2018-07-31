FROM alpine:3.7
LABEL maintainer "Kazuya Takei<attakei@gmail.com>"

RUN apk add --no-cache nodejs python3 \
    && pip3 install docutils-ast-writer \
    && npm i -g textlint textlint-plugin-rst textlint-rule-preset-japanese \
    && mkdir -p /app/content

WORKDIR /app

COPY .textlintrc /app/
ENTRYPOINT ["textlint"]
CMD ["."]

