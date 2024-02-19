FROM ubuntu as stage1

WORKDIR /data

RUN touch abcd.txt

# stage2 

FROM ubuntu as stage2

COPY --from=stage1 /data /data

WORKDIR /data

RUN echo "Hello World">>abcd.txt

FROM alpine

COPY --from=stage2 /data /data 

WORKDIR /data 

CMD [ "cat","abcd.txt" ]







