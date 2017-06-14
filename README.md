# Docker Static Web Server

This image is based on [fnichol/docker-uhttpd](https://github.com/fnichol/docker-uhttpd) which will only serve static html file with "OK"
The reason of creating this image is to have a small container in AWS ECS that will keep the cluster healthy in case you have containers with no http in your cluster like FluentD for example.

## Getting the Image

		docker pull orasws/staticwebserver

## Usage

To run a simple detached container:

		docker run -d -p 8085:80 orasws/staticwebserver


## License
MIT (see [License.txt][license])