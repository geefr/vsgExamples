set(SOURCES
    vsgimgui_rendertotexture_example.cpp
)

add_executable(vsgimgui_rendertotexture_example ${SOURCES})

target_link_libraries(vsgimgui_rendertotexture_example vsgImGui::vsgImGui vsg::vsg)

if (vsgXchange_FOUND)
    target_compile_definitions(vsgimgui_rendertotexture_example PRIVATE vsgXchange_FOUND)
    target_link_libraries(vsgimgui_rendertotexture_example vsgXchange::vsgXchange)
endif()

install(TARGETS vsgimgui_rendertotexture_example RUNTIME DESTINATION bin)
