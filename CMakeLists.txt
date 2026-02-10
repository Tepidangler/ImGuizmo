project(ImGuizmo)

include_directories(BEFORE
                    "${ImGUI_SOURCE_DIR}"
                    )

add_library(ImGuizmo STATIC
        ImGuizmo.h
        ImSequencer.cpp
        ImSequencer.h
        ImZoomSlider.h
        GraphEditor.cpp
        GraphEditor.h
        ImCurveEdit.cpp
        ImCurveEdit.h
        ImGradient.cpp
        ImGradient.h
        ImGuizmo.cpp
)

set_property(TARGET ImGuizmo PROPERTY
        MSVC_RUNTIME_LIBRARY "MultiThreaded$<$<CONFIG:Debug>:Debug>")












