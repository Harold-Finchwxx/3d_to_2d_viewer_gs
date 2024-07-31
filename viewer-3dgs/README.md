## install
1. ubuntu20 安装 ros neotic
2. [3d gaussian splatting](https://github.com/graphdeco-inria/gaussian-splatting)里的`diff_gaussian_rasterization`
3. 安装gsviewer/requirements.txt
4. 安装rospy

## test

### 测试模型渲染

```shell
cd gsviewer
python main.py --file_path <PATH-TO-YOUR-PLY-DIR>/xxx.ply
# e.g.
python main.py --file_path <YOUR-DIR>/models/3dgs/qz11/il_env.ply
```

### 测试ros通讯

1. 终端1

    ```shell
    roscore
    ```

2. 终端2

    ```shell
    cd gsviewer
    python main_ros.py
    ```

3. 终端3

    ```
    python test_ros_server.py
    ```

    