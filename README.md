# A fork of esbuild-sass-plugin

This fork allows you to use CSS modules without having to have it auto-inject.

Think of it as using `transform: postcssModules` *with* `type: "css-text"`.

Just set `inject: false` in the `postcssModules` settings.

Get it from npm: esbuild-sass-plugin-ysink.

## shelter Mode

As this plugin was primarily made for use with [uwu/shelter](https://github.com/uwu/shelter),
there is now shelter-specific support in here for
[Scoped APIs](https://discord.com/channels/824921608560181258/824923929138954241/1203121597016440973)
(also see [efcaae6](https://github.com/uwu/shelter/commit/efcaae613963a2039f4ae8106f203914b7227f5e))
to allow it to be possible to have a normal CSS Modules API while having things unload correctly.

To use it set `inject: "shelter"`.