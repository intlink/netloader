# netloader
Easy-over-HTTP file downloader library for Java>7 using Java NIO.
# How-to
1. First import NetFile class `import netloader.NetFile;`
1. Then proceed (e.g. download a zip from somwhere, with unknown size):
```java
if(new NetFile(new File("my/zips/1.zip"), "https://example.com/example.zip", -1).load()) {
   //downloaded
} else {
   //not downloaded
}
```
