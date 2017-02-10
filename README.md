## Parse - A Static Security Scanner
[![Docker Pulls](https://img.shields.io/docker/pulls/rvannauker/psecio-parse.svg)](https://hub.docker.com/r/rvannauker/psecio-parse/) [![Docker Stars](https://img.shields.io/docker/stars/rvannauker/psecio-parse.svg)](https://hub.docker.com/r/rvannauker/psecio-parse/) [![](https://images.microbadger.com/badges/image/rvannauker/psecio-parse:latest.svg)](https://microbadger.com/images/rvannauker/psecio-parse:latest) [![GitHub issues](https://img.shields.io/github/issues/RichVRed/docker-psecio-parse.svg)](https://github.com/RichVRed/docker-psecio-parse) [![license](https://img.shields.io/github/license/RichVRed/docker-psecio-parse.svg)](https://tldrlegal.com/license/mit-license)

Docker container to install and run psecio-parse

### Installation / Usage
1. Install the rvannauker/psecio-parse container:
```bash
docker pull rvannauker/psecio-parse
```
2. Run psecio-parse through the psecio-parse container:
```bash
sudo docker run --rm --volume $(pwd):/workspace --name="psecio-parse" "rvannauker/psecio-parse" -vvv scan {destination}
```

### Download the source:
To run, test and develop the PSECIO-PARSE Dockerfile itself, you must use the source directly:
1. Download the source:
```bash
git clone https://github.com/RichVRed/docker-psecio-parse.git
```
2. Build the container:
```bash
sudo docker build --force-rm --tag "rvannauker/psecio-parse" --file psecio-parse.dockerfile .
```
3. Test running the container:
```bash
 $ docker run rvannauker/psecio-parse --help
```