FROM node:12-alpine
LABEL version="1.0"
ENV FOO=/app
WORKDIR ${FOO}
COPY . .
ADD test.txt relativeDir/
RUN yarn install --production
CMD ["node", "src/index.js"]
ARG tag_arg
LABEL tag = ${tag_arg}
