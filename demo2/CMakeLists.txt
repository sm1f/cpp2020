# Add executable called "helloDemo" that is built from the source files
# "demo.cpp" and "demo_b.cxx". The extensions are automatically found.
add_executable (helloDemo2 demo.cpp demo_b.cpp)

# Link the executable to the Hello library. Since the Hello library has
# public include directories we will use those link directories when building
# helloDemo2
target_link_libraries (helloDemo2 LINK_PUBLIC Hello)
