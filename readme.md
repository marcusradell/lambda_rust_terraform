# Lambda Rust Terraform

## build code

```sh
docker run --rm \
    -v ${PWD}:/code \
    -v ${HOME}/.cargo/registry:/root/.cargo/registry \
    -v ${HOME}/.cargo/git:/root/.cargo/git \
    softprops/lambda-rust
```

Reference: https://github.com/softprops/lambda-rust

## deploy

Zip should already exist in the `target` folder. Use the aws cli to upload.

## inspirations and references

The source code I started with:
https://github.com/softprops/serverless-aws-rust-http

Some instructions:
https://github.com/awslabs/aws-lambda-rust-runtime
