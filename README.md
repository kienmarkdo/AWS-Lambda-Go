# AWS-Lambda-Go
A basic AWS Lambda function written in Go.

Tutorial steps followed: https://www.youtube.com/watch?v=13rnse0zYK8
    - NOTE: Select "Amazon Linux 2023" in Runtime settings while creating the lambda
Code used: https://docs.aws.amazon.com/lambda/latest/dg/golang-handler.html

JSON input:
```json
{
  "name": "Jane"
}
```
Console commands (Windows 11 Powershell):
```console
$env:GOOS="linux"
$env:GOARCH="amd64"
dir env:  // this is to check whether the env variables have been set
go build -o bootstrap main.go
```
Then zip the bootstrap file and upload the ZIP to the lambda.
