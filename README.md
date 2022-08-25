# minimal_ros2_example
## Set-up

```
mkdir -p example_ws/src
cd example_ws/src
git clone https://github.com/InigoMoreno/minimal_ros2_example.git

rosdep install -iy --from-paths .

cd ..
colcon build --symlink-install
source install/setup.bash
```

## Bug

Open example_ws/src in vscode
Look at file `minimal_ros2_example.py`
You should see that the custom msg Colour has no syntax higlighting or field autocompletion, but the std msg Color RGBA does.
