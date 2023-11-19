# mac-new
Things to do when setting up a new Mac

## 删除自带ABC输入法
sudo open ~/Library/Preferences/com.apple.HIToolbox.plist

接着输入密码即可打开 com.apple.HIToolbox.plist 文件。（打开 .plist 文件需要安装有 Xcode 或者 PlistEdit Pro（可免费试用））

依次点开 Root - AppleEnabledInputSources ，会看到一列 item ，找到其中 KeyboardLayout Name 为 ABC 的那一列，将整列 item 删掉，然后 command + S 保存。

注意1：重启的时候确保删掉的item没有重新出现，如果没及时重启，而进行了切换应用、输入法，item可能还会再出来，重启就没用了，需要再次先删掉。搜狗输入法的“自动切换到英文状态”可能对此有影响（未验证），可以临时关掉。

补充解决方案：sudo open ~/Library/Preferences/ 找到 com.apple.HIToolbox.plist 文件，右键 显示简介 - 勾选已锁定，就不会恢复出现删掉的item了，重启即可。

重启电脑，打开键盘设置，就可以看到系统自带的 ABC 输入法已经被删掉了。

注意2：删掉ABC输入法后已知问题，会造成偏好设置 -> 网络设置里面修改网络参数的时候一点输入框就卡死，重新添加ABC即可。

恢复ABC输入法，重新添加ABC输入法即可。

<img width="800" alt="image" src="https://github.com/ningxiaowa/mac-new/assets/13115229/57daf00f-a4ef-456f-849d-578a673c70d5">
