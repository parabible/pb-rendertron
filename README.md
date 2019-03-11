# pb-rendertron
Rendertron docker image to do some SSR substition

## Instructions

Docker makes everything very difficult. So these instructions might go over your head.

First you're going to want to build the image.

```
docker build -t pb-rendertron/slim .
```

Then you're going to want to run it:

```
docker run --name pb-rendertron -p 80:80 pb-rendertron/slim
```
