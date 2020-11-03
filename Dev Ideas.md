Available gfx.canvas.azure.backends;

Windows XP+: d3d(?) (Direct3D), macOS: cg (Quartz), HwAc Fallback: skia (Skia), SfRn Fallback 2: cairo (Cairo)

Available gfx.content.azure.backends;

Windows Vista+: direct2d1.1 (Direct2D), macOS: cg (Quartz), HwAc Fallback: skia (Skia), SfRn Fallback 2: cairo (Cairo)

D2/3d = skia > cg > cairo

More:

javascript.options.shared_memory;true - Leverages second thread to share memory allocated for JS with; disabled in 2018 due to Spectre, and currently in process of being re-enabled, so leave alone

Future:

media.ffvpx.enabled;true (FF 76+) - Leverages GPU to render VP9; no effect for MP4
dom.webgpu.enabled;true (FF 68+?) - Currently unstable; do not use
