



# How to build a whl for use

- 编译环境是 gcc (GCC) 12.2.0，Ubuntu 20.04.5，其他环境也许是可以的，但是我们没有验证过。

python3.8  -m pip wheel ./python --wheel-dir=/nishirong/TRITON_PADDLE/built_wheel_by_nsr --no-deps
python3.8 -m pip install /nishirong/TRITON_PADDLE/built_wheel_by_nsr/triton-2.1.0-cp38-cp38-linux_x86_64.whl 

wheel-dir 为whl包产生的文件夹路径

# Use with PADDLE
- Set `export TRITON_USE_PADDLE=TRUE` to use TRITON with PADDLE.
