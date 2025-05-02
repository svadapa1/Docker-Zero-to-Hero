###########################################
# BASE IMAGE
###########################################



FROM openjdk:11

RUN javac Main.java

ENV GO111MODULE=off

COPY . .

RUN CGO_ENABLED=0 go build -o /app .

ENTRYPOINT ["/app"]

