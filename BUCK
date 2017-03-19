include_defs('//BUCKAROO_DEPS')

cxx_library(
  name = 'toluapp',
  header_namespace = '',
  exported_headers = subdir_glob([
    ('include', '*.h'),
  ]),
  srcs = glob([
    'src/lib/**/*.c',
  ]),
  visibility = [
    'PUBLIC'
  ],
  deps = BUCKAROO_DEPS,
)

cxx_library(
  name = 'toluappbin',
  header_namespace = '',
  exported_headers = subdir_glob([
    ('include', '*.h'),
  ]),
  srcs = glob([
    'src/bin/**/*.c',
  ]),
  visibility = [
    '//...'
  ],
  deps = BUCKAROO_DEPS + [
    ':toluapp',
  ],
)
