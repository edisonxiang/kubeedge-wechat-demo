# Start from golang v1.11 base image
FROM golang:1.11

COPY . $GOPATH/src/github.com/edisonxiang/kubeedge-wechat-demo/kubeedge-wechat-app

# Set the Current Working Directory inside the container
WORKDIR $GOPATH/src/github.com/edisonxiang/kubeedge-wechat-demo/kubeedge-wechat-app

# Install the package
RUN CGO_ENABLED=0 GO111MODULE=off go install -v

# Run the executable
CMD ["kubeedge-wechat-app"]
