# Rendertron in Docker for Parabible

If you want information on rendertron, go here: https://github.com/GoogleChrome/rendertron/. This repo gets rendertron in a docker instance (which is no longer really supported). Also, it's worth noting this handy Express middleware that helps make use of a rendertron instance: https://www.npmjs.com/package/rendertron-middleware.

The distinctive feature that makes this a *parabible* rendertron is that it includes the SBL Biblit font from https://www.sbl-site.org/educational/BiblicalFonts_SBLBibLit.aspx.

# Instructions

Docker makes everything very difficult. So hold onto your hats everyone.

First you're going to want to build the image:

```
docker build -t pb-rendertron/slim .
```

Then you're going to want to run it:

```
docker run --name pb-rendertron -p 80:80 pb-rendertron/slim
```
