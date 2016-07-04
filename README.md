# Redis-S3-Backup
Python script to back up your Redis RDB file to S3

## Installation
`$ pip install redis_s3_backup`

## Usage
```
redis_s3_backup
  --directory DIRECTORY_CONTAINING_RDB_FILE
  --bucket S3_BUCKET_NAME
  --profile AWS_PROFILE_NAME
```

### Redis Directory
This is the directory in which the `dump.rdb` file is located. If you installed Redis by compiling it, this would look like `~/redis-3.2.1` (if you extracted the tar file in your home directory).

### S3 Bucket Name
This is the AWS S3 bucket which will contain your backups.

### AWS Profile Name
This is the profile to be used, for instance if your shared credentials file looks like this:
```
$ cat ~/.aws/credentials
[AWS_PROFILE_NAME]
aws_access_key_id=YOUR_ACCESS_KEY_ID
aws_secret_access_key=YOUR_SECRET_ACCESS_KEY
```
Then use `--profile` to specify that your profile name is `AWS_PROFILE_NAME`
