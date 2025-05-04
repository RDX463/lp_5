## For running the HPC code REQUIREMENT: MingW64 (latest version g++ (MinGW-W64 x86_64-msvcrt-posix-seh, built by Brecht Sanders, r1) 15.1.0) 

### Installation

## Download MinGW-w64

## Go to: https://github.com/brechtsanders/winlibs_mingw/releases/tag/15.1.0posix-12.0.0-msvcrt-r1

## Download the latest MinGW-w64 standalone build.

## 2. Extract and Configure

## Extract to a folder like: C:\mingw-w64

## Add C:\mingw-w64\bin to your system PATH.

### Run this

```bash
g++ -fopenmp <filename>.cpp -o <filename>.exe
```

```bash
<>filename>.exe
```

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🧪 How to Run HPC CUDA codes

### 1. Open the correct terminal in folder where is your code file

```bash
nvcc <filename>.cu -o <filename>.exe
```
### 2. After Compiling run this

```bash
<filename>.exe
```
### 3. Enter the inputs to run the code

## Note:

### If gets error like this

```bash
nvcc fatal   : Cannot find compiler 'cl.exe' in PATH
```
### then do this
### 1. install cuda toolkit
### 2. find this "C:\Program Files\Microsoft Visual Studio\2022\Community\VC\Tools\MSVC\14.38.33130\bin\Hostx64\x64\cl.exe"
### 3. Enter this in terminal:
```bash
set PATH=C:\Program Files\Microsoft Visual Studio\2022\Community\VC\Tools\MSVC\14.38.33130\bin\Hostx64\x64;%PATH%
```
### 4. Run command
```bash
nvcc <filename>.cu -o <filename>.exe
```




