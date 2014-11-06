# Nodeboxtest

Test image for BusyBox based nodejs-runtime for sirile/nodebox. Base image is built on progrium/busybox.

Uses node.js runtime v0.10.33. 

## Usage

### TL;DR

```
sudo docker run --name filebox sirile/filebox
sudo docker run --rm --name=nodeboxtest -p 3000:3000 --volumes-from filebox -ti sirile/nodeboxtest
```

### Step by step

First you need to have the filebox volume container created:

```
sudo docker run --name filebox sirile/filebox
```

Then you can run the very basic express based application that outputs hello world:

```
sudo docker run --rm --name=nodeboxtest -p 3000:3000 --volumes-from filebox -ti sirile/nodeboxtest
```

After that it should be available at the address http://<host>:3000. You can exit with CTRL+C.

## Author

Ilkka Anttonen. Comments and suggestion are welcome.
