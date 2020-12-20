gfx.canvas.azure.backends / gfx.content.azure.backends:

D2/3d = skia > cg > cairo

More:

javascript.options.shared_memory;true - Leverages second thread to share memory allocated for JS with; disabled in 2018 due to Spectre, and currently in process of being re-enabled by Mozilla, so leave alone

Future:

media.ffvpx.enabled;true (FF 76+) - Leverages GPU to render VP9; no effect for MP4
dom.webgpu.enabled;true (FF 68+?) - Currently unstable; do not use
