FROM golang:1.11
#copy and build and install btcwallet
WORKDIR /go/src/github.com/btcsuite/btcwallet
COPY . .
RUN go get -u github.com/Masterminds/glide
RUN glide install
RUN go install . ./cmd/...
RUN mkdir -p /root/.btcwallet
RUN touch /root/.btcwallet/btcwallet.conf
#copy source code  
WORKDIR /go/src/github.com/btcsuite/btcd
COPY ./btcd/ .
#build and install btcd
WORKDIR /go/src/github.com/btcsuite/btcd
RUN glide install
RUN go build
RUN env GO111MODULE=on go install . ./cmd/...