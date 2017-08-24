project('curlcpp', 'cpp', version : '1.0+git20170822', license : 'MIT')

src = ['src/curl_easy.cpp', 'src/curl_header.cpp',
    'src/curl_global.cpp', 'src/curl_form.cpp',
    'src/curl_multi.cpp', 'src/curl_share.cpp',
    'src/curl_info.cpp', 'src/curl_cookie.cpp',
    'src/curl_exception.cpp', 'src/cookie.cpp',
    'src/cookie_date.cpp', 'src/cookie_time.cpp',
    'src/cookie_datetime.cpp'
]

curl_dep = dependency('libcurl', required: true)
incdir = include_directories('include')

curlcpplib = library('curlcpp', src, include_directories: incdir, dependencies: curl_dep)

curlcpp_dep = declare_dependency(link_with : curlcpplib,
  include_directories : incdir)

