FROM quay.io/souravkl11/raganork:multidevice

ADD https://api.github.com/repos/Sjshskdhd/raganork-md/git/refs/heads/main version.json
RUN git clone -b main https://github.com/Sjshskdhd/raganork-md /rgnk
WORKDIR /rgnk
ENV TZ=Asia/Kolkata
RUN yarn install --ignore-engines --network-concurrency 1
EXPOSE 3000
CMD ["node", "index.js"]
