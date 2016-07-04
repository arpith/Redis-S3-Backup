# Redis-S3-Backup
Python script to back up your Redis RDB file to S3

## Installation
`$ pip install redis_s3_backup`

## Usage
`redis_s3_backup --directory DIRECTORY_CONTAINING_RDB_FILE --bucket S3_BUCKET_NAME`

### Redis Directory
This is the directory in which the dump.rdb file is located. If you installed Redis by compiling it, this would look like `~/redis-3.2.1` (if you extracted the tar file in your home directory).
