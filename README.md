# bash-s3
AWS S3 get and put in bash using instance IAM role credential. 

## Prerequisite
* curl
* openssl
* hmac_sha256

## S3 Get

Usage: `s3get.sh <bucket> <filePath> <destination>`

```
./s3get.sh my-s3bucket foo/bar.txt bar.txt
```

This will download s3://my-s3bucket/foo/bar.txt to ./bar.txt


## S3 Put

Usage: `s3put.sh <bucket> <parent/path> <source>`

```
./s3put.sh my-s3bucket foo ./bar.txt 
```

This will upload ./bar.txt to s3://my-s3bucket/foo/bar.txt
