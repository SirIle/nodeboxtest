# Nodeboxtest

Test image for BusyBox based nodejs-runtime for sirile/nodebox. Base image is built on progrium/busybox.

Uses node.js runtime v0.10.33. 

## Usage

Includes a very basic express based application that outputs hello world. Can be run with:

```
sudo docker run --rm -p 3000:3000 -ti sirile/nodeboxtest
```

## Author

Ilkka Anttonen. Comments and suggestion are welcome.
