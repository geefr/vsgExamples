add_subdirectory(vsginput)

if (vsgImGui_FOUND)
    add_subdirectory(vsgimgui_example)
    add_subdirectory(vsgimgui_rendertotexture_example)
endif()
