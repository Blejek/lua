cmake_minimum_required(VERSION 3.7)

project( LuaLib )

# The recommended way to collect sources in variable by explicitly specifying the source files
set  (LUA_RUNTIME_SOURCES
"lapi.c"
"lcode.c"
"lctype.c"
"ldebug.c"
"ldo.c"
"ldump.c"
"lfunc.c"
"lgc.c"
"llex.c"
"lmem.c"
"lobject.c"
"lopcodes.c"
"lparser.c"
"lstate.c"
"lstring.c"
"ltable.c"
"ltm.c"
"lundump.c"
"lvm.c"
"lzio.c"
"lauxlib.c"
"lbaselib.c"
"lcorolib.c"
"ldblib.c"
"liolib.c"
"lmathlib.c"
"loadlib.c"
"loslib.c"
"lstrlib.c"
"ltablib.c"
"lutf8lib.c"
"linit.c"
)
  
add_library( LuaLib ${LUA_RUNTIME_SOURCES} )

target_include_directories ( LuaLib PUBLIC "${PROJECT_SOURCE_DIR}/src")
