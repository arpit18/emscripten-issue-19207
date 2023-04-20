# emscripten-issue-19207
Isolated repro steps for https://github.com/emscripten-core/emscripten/issues/19207

## Version of emscripten/emsdk
Version of emscripten/emsdk:
emcc (Emscripten gcc/clang-like replacement + linker emulating GNU ld) 3.1.33 (c1927f2)
clang version 17.0.0 (https://github.com/llvm/llvm-project 671eeece457f6a5da7489f7b48f7afae55327b8b)
Target: wasm32-unknown-emscripten
Thread model: posix

## Operating System
Windows 10 Pro
Version 		: 21H2
OS Build 		: 19044.2486

## Steps :
- Open `CMD`
- Set up emscripten environment variables using the steps given at [Emscripten - Download and Install](https://emscripten.org/docs/getting_started/downloads.html)
- Switch to **emscripten-issue-19207** folder
- Run : build.bat
	- Runs Successfully
- Run : build_with_quotes.bat
	- Fails with the error : `<path-to-emsdk>\python\3.9.2-nuget_64bit\python.exe can't open file '<path-to-folder>\emscripten-issue-19207\emcc.py': [Errno 2] No such file or directory`
