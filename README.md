``` bash
repo init -u https://github.com/android-rockchip/build.git -b master -m rockchip-s-release.xml
repo sync -d --no-clone-bundle --no-tags -j16

chmod +x build.sh

source build/envsetup.sh
lunch orangepi5-userdebug
./build.sh -AUKu
```

Based on Radxa sources repository - https://gitlab.com/rockchip_android_s
