project('Adafruit_MCP4725', 'cpp',
    version: '2.0.2',
)

adafruit_busio_dep = subproject('Adafruit_BusIO').get_variable('adafruit_busio_dep')
adafruit_mcp4725_lib = static_library('adafruit_mcp4725',
    sources: [
        'Adafruit_MCP4725.cpp',
    ],
    cpp_args: [
        '-std=c++17',
    ],
    dependencies: [
        adafruit_busio_dep,
    ],
)

adafruit_mcp4725_dep = declare_dependency(
    link_with: adafruit_mcp4725_lib,
    include_directories: '.',
    dependencies: [
        adafruit_busio_dep,
    ],
)