# AllegroStarterProject
In order to setup Allegro 4.4.2 with Visual Studio, follow the given steps:
1. Download Allegro binaries from http://cdn.allegro.cc/file/library/allegro/4.4.2/allegro-4.4.2-msvc-10.0.zip
2. Extract the files to C:\ such that folder tree looks like:
```       
       C:
       |
       |_ allegro
            |
            |_ bin
            |_ include
            |_ lib
  
```
3. Add `C:\allegro\bin` to PATHS in environment variables.
4. Create a new Visual Studio Console C++ project.
5. Go to properties of the project and perform following changes
    - **VC++ Directories  > Include Directories** add `C:\allegro\include`
    - **VC++ Directories  > Library Directories** add `C:\allegro\lib`
    - **Linker > Input** add `allegro-4.4.2-md.lib`
    - **Linker  > System > Subsystem** set to `Windows`
6. You're ready to go!! Use the .cpp file provided in the repo for a testing the project (Project might not build if you don't have proper test code).
