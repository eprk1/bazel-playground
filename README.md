export CC=/opt/cross/el8.5-x86_64/gcc-12.1.0/bin/gcc
export CXX=/opt/cross/el8.5-x86_64/gcc-12.1.0/bin/g++

bazel build //app:app \
  --action_env=CC=$CC \
  --action_env=CXX=$CXX
