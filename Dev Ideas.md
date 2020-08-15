Current gfx.canvas.azure.backends / gfx.content.azure.backends; cg,skia,cairo

Available gfx.canvas.azure.backends;

Windows XP+: d3d(?) (Direct3D), macOS: cg (Quartz), HwAc Fallback: skia (Skia), SfRn Fallback 2: cairo (Cairo)

Available gfx.content.azure.backends;

Windows Vista+: direct2d1.1 (Direct2D), macOS: cg (Quartz), HwAc Fallback: skia (Skia), SfRn Fallback 2: cairo (Cairo)

D2/3d = skia > cg > cairo

More:

javascript.options.shared_memory;true - Leverages second thread to share memory allocated for JS with; disabled in 2018 due to Spectre, and currently in process of being re-enabled, so leave alone
extensions.blocklist.enabled;false - Disables the addon blocklist updating system, freeing resources (compromises on security)
extensions.pocket.enabled;false - Disables the Pocket feature, freeing resources (disabled on PM, WF, so no need)
* gfx.xrender.enabled;true - Switches page rendering from the Firefox process to the X11 process; results in slightly better video and page rendering performance


Future:

media.ffvpx.enabled;true (FF 76+) - Leverages GPU to render VP9; no effect for MP4
dom.webgpu.enabled;true (FF 68+?) - Currently unstable; do not use
