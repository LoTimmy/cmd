`FUSE-based file system backed by Amazon S3`

```
shell> sudo apt-get install automake autotools-dev fuse g++ git libcurl4-gnutls-dev libfuse-dev libssl-dev libxml2-dev make pkg-config
shell> git clone https://github.com/s3fs-fuse/s3fs-fuse.git
shell> cd s3fs-fuse
shell> ./autogen.sh
shell> ./configure
shell> make
shell> sudo make install
```

```
shell> brew tap homebrew/fuse
shell> brew install s3fs
```

```
shell> echo MYIDENTITY:MYCREDENTIAL > /etc/passwd-s3fs
shell> chmod 600 /etc/passwd-s3fs
shell> s3fs mybucket /path/to/mountpoint -o passwd_file=/etc/passwd-s3fs

```

`/etc/fuse.conf`

```
# Allow non-root users to specify the allow_other or allow_root mount options.
user_allow_other
```

```
s3fs Your_Bucket_Name -o allow_other You_Dir_Full_Path -o passwd_file=Password_Full_Path -o use_cache=/tmp -o ahbe_conf=Metadata_Config_Full_Path -o default_acl=public-read
```

```
fusermount -u /path/to/mountpoint
```


- https://github.com/s3fs-fuse/s3fs-fuse.git
