project(
	'samurai',
	'c',
	version: '0.1.0',
	license: 'GPL3',
	meson_version: '>=0.48.0',
	default_options: [
		'c_std=c99',
		'warning_level=3',
		'buildtype=debugoptimized',
		'default_library=static',
	],
)

src = files([
	'build.c',
	'deps.c',
	'env.c',
	'graph.c',
	'htab.c',
	'log.c',
	'parse.c',
	'samu.c',
	'scan.c',
	'tool.c',
	'tree.c',
	'util.c',
])

libsamu = library('samu', src)

libsamu_dep = declare_dependency(
	link_with: [libsamu],
	include_directories: include_directories('.'),
)
