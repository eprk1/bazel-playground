export CC=/opt/cross/el8.5-x86_64/gcc-12.1.0/bin/gcc
export CXX=/opt/cross/el8.5-x86_64/gcc-12.1.0/bin/g++

bazel build //app:app \
  --action_env=CC=$CC \
  --action_env=CXX=$CXX


Milestones
Build and render a Sun–Earth system.
Add Newtonian N-body gravity.
Add camera movement and simulation controls.
Add orbital trails.
Load scenarios from JSON.
Add collisions and body merging.
Parallelize force calculations.
Add Barnes–Hut optimization for thousands of bodies.
Add benchmarks and tests.
Package Linux and macOS binaries with Bazel.