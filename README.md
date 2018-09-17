# AWS icon set for plantuml

Inspired by [plantuml-icon-font-sprites](https://github.com/tupadr3/plantuml-icon-font-sprites) I downloaded 
[AWS Simple Icons](https://aws.amazon.com/architecture/icons/), extracted, and made ``.puml`` files.

Both resized images and plantuml sprites are available.

## How to use

```
!define AWS_SPRITESPATH https://raw.githubusercontent.com/jballe/plantuml-aws-icons/master/sprites
!includeurl AWS_SPRITESPATH/compute/ec2.puml
```

For each icon there is defined variables for three images, a greyscale and a color version, and a block and what., All resized to 48x48 pixels.

```
component "s3 b/w \nAWSIMG_S3BUCKET_B" as bucket_b
component "s3 gray \nAWSIMG_S3BUCKET_G" as bucket_g
component "S3 color \nAWSIMG_S3BUCKET_C" as bucket_c
```

There is also defined a plantuml native sprite based on the black and white image.

```
component "s3 sprite \n<$s3bucket>" as bucket
```

