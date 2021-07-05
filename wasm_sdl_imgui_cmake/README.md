# wasm_sdl_imgui_cmake

- ## 0.source

  [schteppe/imgui-wasm: imgui/wasm boilerplate (github.com)](https://github.com/schteppe/imgui-wasm)

- ## **1.development_wasm(Emscripten)**

  - **1.0**

    make sure you have required softs/environments

    确保你安装了必要的软件和环境

    vscode, Emscripten

    vscode extensions: cmake cmake tools

  - **1.1**

    1.1.1

    set the toolchain in vscode cmake extension

    设置工具栏

    ![image-20210705171613749](https://hanbaoaaa.xyz/tuchuang/images/2021/07/05/image-20210705171613749.png)

    > [vscode-cmake-tools/kits.md at develop · microsoft/vscode-cmake-tools (github.com)](https://github.com/microsoft/vscode-cmake-tools/blob/develop/docs/kits.md)

    1.1.2

    set the cmake generator

    设置generator

    ![image-20210705171708520](https://hanbaoaaa.xyz/tuchuang/images/2021/07/05/image-20210705171708520.png)

  - **1.2**

    use vscode open this folder,

    **ctrl+shift+p**  open the palette, cmake config, cmake debug

    使用vscode 打开这个文件夹

    命令面板 执行cmake config 和cmake debug

  - **1.3** 

    files will be generated in build

    文件生成 到build文件夹

    ![image-20210705172106548](https://hanbaoaaa.xyz/tuchuang/images/2021/07/05/image-20210705172106548.png)

  - **1.4**

    run python server to test

    运行服务器来测试

    with Python 2: ```python -m SimpleHTTPServer 8080```

    with Python 3: ```python -m http.server 8080```

  - **1.5**

    online demo:

    [ImGUI / WASM / WebGL demo (hanbaoaaa.xyz)](https://hanbaoaaa.xyz/apps/WasmDemo/)

- ## 2.development_native

  - **tested:** windows

  - **2.1**

    install conan

  - **2.2**

    run **shell_conan.sh** 

    windows can use git_bash to run .sh

  - **2.3**

    follow the steps in 1.1.2 and 1.2

  


