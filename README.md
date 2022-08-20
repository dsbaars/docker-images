# Docker Images
Repo for fixed and/or improved docker images to prevent many smaller repositories.


## polar-eclair-multiarch

Container to be used with [Polar](https://lightningpolar.com/). 
The original container only supported `amd64`, modified it to run it on `arm64` as well.

Example:
`docker buildx build --platform=linux/arm64,linux/amd64 --build-arg ECLAIR_VERSION=0.7.0 --tag dsbaars/polar-eclair:0.7.0 --output type=registry .`