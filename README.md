# mac-new
Things to do when setting up a new Mac

## 删除自带ABC输入法
sudo open ~/Library/Preferences/com.apple.HIToolbox.plist

接着输入密码即可打开 com.apple.HIToolbox.plist 文件。（打开 .plist 文件需要安装有 Xcode 或者 PlistEdit Pro（可免费试用））

依次点开 Root - AppleEnabledInputSources ，会看到一列 item ，找到其中 KeyboardLayout Name 为 ABC 的那一列，将整列 item 删掉，然后 command + S 保存。

重启电脑，打开键盘设置，就可以看到系统自带的 ABC 输入法已经被删掉了。

恢复ABC输入法

重新添加ABC输入法即可

<img width="800" alt="image" src="https://github.com/ningxiaowa/mac-new/assets/13115229/57daf00f-a4ef-456f-849d-578a673c70d5">
