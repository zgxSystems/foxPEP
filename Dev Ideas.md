Current gfx.canvas.azure.backends / gfx.content.azure.backends; cg,skia,cairo

Available gfx.canvas.azure.backends;

Windows XP+: d3d(?) (Direct3D), macOS: cg (Quartz), Linux: opengl(?) (OGL), HwAc Fallback: skia (Skia), SfRn Fallback 2: cairo (Cairo)

Available gfx.content.azure.backends;

Windows Vista+: direct2d1.1 (Direct2D), macOS: cg (Quartz), Linux: xr(?) (XRender), HwAc Fallback: skia (Skia), SfRn Fallback 2: cairo (Cairo)

More:

extensions.blocklist.enabled;false - Disables the addon blocklist updating system, freeing resources
extensions.pocket.enabled;false - Disables the Pocket feature, freeing resources (disabled on PM, WF, so no need)
gfx.xrender.enabled;true - Switches page rendering from the Firefox process to the X11 process, potentially freeing resources


Future:

media.ffvpx.enabled;true (FF 76+) - Leverages GPU to render VP9; no effect for MP4
dom.webgpu.enabled;true (FF 68+?) - Currently unstable; do not use

javascript.options.shared_memory;true - Leverages second thread / core to crunch JS (disabled on FF, WF, enabled on PM, TFF)
