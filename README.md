# Swift for TensorFlow in Ubuntu Docker

## Download

(Specified in every version folder)

Download Swift for TensorFlow and place it in the same folder with Dockerfile

```
cd to folder path where Dockerfile and Swift are placed:

docker build -t tensorswift .
```

## Run
```
docker run -it --privileged tensorswift
```
## Check

Inside Swift command line:
```
import TensorFlow
```
