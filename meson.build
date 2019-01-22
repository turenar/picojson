project('picojson', 'cpp')

compiler_arguments = []
if get_option('int64')
	compiler_arguments += ['-DPICOJSON_USE_INT64']
endif
if get_option('use_locale')
	compiler_arguments += ['-DPICOJSON_USE_LOCALE']
endif

picojson_dep = declare_dependency(
	include_directories: include_directories('.', is_system: true),
	compile_args: compiler_arguments)

