project(mri_parse_sdcmdir)

include_directories(${FS_INCLUDE_DIRS})

add_executable(mri_parse_sdcmdir mri_parse_sdcmdir.c)
target_link_libraries(mri_parse_sdcmdir utils)

add_test_script(NAME mri_parse_sdcmdir_test SCRIPT test_mri_parse_sdcmdir DEPENDS mri_parse_sdcmdir)

install(TARGETS mri_parse_sdcmdir DESTINATION bin)
