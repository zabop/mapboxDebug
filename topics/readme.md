# t0

Save [`t0.html`](https://github.com/zabop/mapboxDebug/blob/master/topics/t0.html) and open it in a browser. Make sure you see a blue square.

Edit the file to achieve the following.

1. Make the square red
2. Make the square blue and somewhat transparent.

# t1

Take a look at [`t1.html`](https://github.com/zabop/mapboxDebug/blob/master/topics/t1.html).

3. Can you explain why the colour is [something like this](https://en.wikipedia.org/wiki/Blue-green)?

I don't have a good answer for number 4., and I find number 5. quite buffling. Having a think about them might benefit your future debugging skills.

4. Now look at `raster-color-range` ([docs](https://docs.mapbox.com/style-spec/reference/layers/#paint-raster-raster-color-range)) section. Change it to: `"raster-color-range": [0 / normalizer, 258 / normalizer]`. Why does the square have the colour it has?

5. In addition to the `raster-color-range` change in step 4, load `R155.webp` instead of `R156.webp` (this is a webp with all RGB values set to 155,0,0). Why do we still have a squre shown?

I tried to have a satisfactory answer to 4. and 5. via a drawing, I didn't get there. Here is the drawing nevertheless:

![](https://raw.githubusercontent.com/zabop/mapboxDebug/refs/heads/master/topics/plot.jpg)

# t2

Take a look at [`t2.html`](https://github.com/zabop/mapboxDebug/blob/master/topics/t2.html).

6. Again, we are loading [R156.webp](https://raw.githubusercontent.com/zabop/mapboxDebug/master/webps/R156.webp), which is a webp with all pixels' RGB triplet set to (156,0,0). `"raster-color-mix"` is set to `[0, 1, 0, 0]`. While leaving `"raster-color-mix"` as it is, modify code so a red square shows up.
