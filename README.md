# CORPCA-OF
Code base for video foreground background separation algorithm: CORPCA-OF

Please look up https://github.com/huynhlvd/corpca-of for more info.

1. Open CMake GUI
2. Drag and drop CmakeLists.txt from the "CORPCA-OF" folder into CMake
3. Select output path, type in "build" after the path
4. Select configure, choose your compiler (VS 2017/2015 etc.)
5. After no errors are present, click generate
6. If you go to the CORPCA-OF folder, you will see a build folder created, open it
7. Open the visual studio project that is created
8. Build the solution
9. Select the project demoCORPCA-OF and set it as start up project
10. Now select "Run"
11. Enter path to the video files (ex D:\TRACK)
12. Enter path where output has to be saved (ex D:\outDataOF)
13. Enter sequence name (Bootstrap, Curtain etc.)
14. Enter the format name (bmp, png etc.)
14. Enter scaling factor (1.0, 0.5, 0.25)
15. Enter rate (1.0, 0.8, 0.6, 0.4, 0.2)
16. Check the output folder that was specified to see the seperated images

NOTE: 
* Inside the output folder, please create folders with names of video sequences. i.e. for every sequence in TRACK, create a new empty folder inside the output path folder (D:\outDataOF)
* Create a folder named prior inside video sequence folder (ex in TRACK)
* For every sequence in TRACK, create a new folder inside the prior folder
Here is a sample folder structure:

- TRACK
    * Bootstrap 
    * Curtain 
    * ...
    * prior 
      + Bootstrap (to be created)
      + Curtain (to be created)
      + ...
- outDataOF
    * Bootstrap (to be created)
    * Curtain (to be created)
    * ...

