Exa
===

Use this container to build linux binaries of [exa](https://the.exa.website).  
  
Currently, exa doesn't publish linux binaries. Here's how you can use this container to build a binary without having to install Rust on your local machine.  

```
docker pull abh1nav/exa:0.8.0
docker run -it --rm -v `pwd`:/output abh1nav/exa:0.8.0
```
  
This will run the container and copy the exa binary into your current working directory.    
