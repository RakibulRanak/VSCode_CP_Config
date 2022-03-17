1.Install c++ extension
2.Install Code Runner
3. Settings > Extensions > Run Code Configuration > Executor Map > paste this--

{
    "window.zoomLevel": 2,
    "code-runner.executorMap": {
    
        "javascript": "node",
        "java": "cd $dir && javac $fileName && java $fileNameWithoutExt",
        "c": "cd $dir && gcc $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
        "cpp": "echo 'Compiling...' && cd $dir && g++ -std=c++17 $fileName  && echo 'Running...' && timeout 1s ./a.out < input.txt > output.txt && echo 'Completed!!'"
    },
    "editor.formatOnSave": true,
    "files.autoSave": "onFocusChange"
}

4. Create a folder
5. Inside create input.txt and output.txt
6. Create Cpp file
7. Layout
8. Save and Run by Ctrl+Alt+N
9. Stop by Ctrl+Alt+M
10. Create a workspace inside the folder by  file > save workspace as...
11. From now , just go inside the folder,open terminal and press code . 


* for mac m1 read this > https://dev.to/ayushpattnaik/running-c-17-on-mac-m1-47cp
