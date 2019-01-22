project('picojson', 'cpp')

compiler_arguments = []
if get_option('int64')
	compiler_arguments += ['-DPICOJSON_USE_INT64']
endif
if get_option('assert')
	compiler_arguments += ['-DPICOJSON_ASSERT']
endif
if get_option('use_locale')
	compiler_arguments += ['-DPICOJSON_USE_LOCALE']
endif

picojson_dep = declare_dependency(
	include_directories: include_directories('.'),
	compile_args: compiler_arguments)

