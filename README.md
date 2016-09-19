modeshape-s3-binary-store
=========================

A custom binary store for ModeShape which stores files in Amazon S3.

*NOTE: The work contained in this project has been [merged](https://github.com/ModeShape/modeshape/pull/1586) into ModeShape.
It is recommended that the version in ModeShape be used rather than this project.*

# Dependencies
This binary store implementation was built for and tested against ModeShape 5.x, it is not meant to be used
with previous versions of ModeShape, especially those which rely on Infinispan.

# Build
This project is built using Maven:
```
mvn install
```

# Configuration
The following system properties must be defined and made available:
aws.accessKeyId  // The Access Key ID portion of AWS access credentials
aws.secretKey    // The Secret Key portion of AWS access credentials
aws.bucket       // The name of the bucket to use in S3, this bucket if created if it does not exist

## Maintainers

* [Bill Branan](https://github.com/bbranan)
