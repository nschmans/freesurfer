project(mris_jacobian)

include_directories(${FS_INCLUDE_DIRS})

add_executable(mris_jacobian mris_jacobian.c)
add_help(mris_jacobian mris_jacobian.help.xml)
target_link_libraries(mris_jacobian utils)

add_test_script(NAME mris_jacobian_posix_test SCRIPT test_fs_posix DEPENDS mris_jacobian)

install(TARGETS mris_jacobian DESTINATION bin)
