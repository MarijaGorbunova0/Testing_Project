How to work with firmware
1. set the workspace for zephyr using this guide 
2. clone in the workspace this repo 
NOTE! before working or compile files don't forget to use virtual environment 
```bash
source .venv/bin/activate
```
3. Compile firmware 

```bash
west build -b stm32l4_icp -- -DBOARD_ROOT=$(pwd)
```

west build - Zephyr build team

-b stm32l4_icp - board: which board we are building for

-- - separator: further arguments for CMake

-DBOARD_ROOT=$(pwd) - where to look for the board: in the current directory (pwd)
