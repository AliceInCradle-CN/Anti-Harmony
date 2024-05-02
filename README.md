# Anti-Harmony
游戏《Alice In Cradle》的反和谐步骤。

## 使用 `dnSpy` 进行反编译修改

### 准备工作

 - [Alice In Cradle 游戏本体](https://cn.aliceincradle.dev/)
 - [dnSpy](https://github.com/dnSpy/dnSpy)
 - Windows 系统

---

1. 下载游戏 `Alice In Cradle` *如果已下载，请跳过此步骤*
   
   访问 [`https://cn.aliceincradle.dev/`](https://cn.aliceincradle.dev/) 并且点击下方图片上的位置：
   
   ![image](https://github.com/AliceInCradle-CN/Anti-Harmony/assets/62281844/ffb0dccd-535d-42d4-ba18-6d6cb1cbae15)

   ![image](https://github.com/AliceInCradle-CN/Anti-Harmony/assets/62281844/846dae58-bf96-4b3f-a256-dc76ae5d790a)

   选择 `Windows`：

   下载压缩包，以方便操作；

   下载之后，将压缩包解压到您喜欢的位置。

   至此，第一步完成。

2. 下载 `dnSpy` *如果已下载，请跳过此步骤*

   访问 [`https://github.com/dnSpy/dnSpy`](https://github.com/dnSpy/dnSpy)，之后，点击右侧的 `Release`；

   找到最新的版本，根据您的 CPU 架构选择 是否为 `Win32` 或 `Win64`；

   下载压缩包；

   下载完成后，将压缩包解压到您喜欢的位置。
   
   至此，第二步完成。

### 通过 `dnSpy` 对游戏 `Alice In Cradle` 进行修改

1. 打开 dnSpy 进行反编译工作

   打开您在 **第二步** 解压完成的文件夹，并运行 `dnSpy.exe`；

   点击 菜单栏 中的 `文件(F) - 打开(O)...`；

   在弹出的对话框中，选择您在 **第一步** 解压的游戏本体目录，在地址栏后面加上 `AliceInCradle_Data\Managed`；

   选择 `Assembly-CSharp.dll` 并且点击 `打开(O)` 按钮；

   ---

   点击 菜单栏 中的 `编辑(E) - 搜索程序集(S)`；

   在右下方的搜索框中粘贴 `FnDrawMosaic` 并且搜索(通常，搜索步骤是自动的，您只需要粘贴就好。)；

   选择搜索结果中的第一个；

   向下滚动到分隔线处；
   
   ![ScreenShot](https://github.com/AliceInCradle-CN/Anti-Harmony/assets/62281844/cf2351a8-bc11-41e4-b917-12f29503498e)

   右键分隔线上方的代码，并点击 `编辑类(C#)...`；

   将 `return true;` 中的 `true` 改为 `false`；

   点击 `编译` 按钮；

   单击上方工具栏的 `保存所有(Ctrl+Shift+S)` 按钮，并且在弹出的窗口中点击 `确定(O)` 按钮。

   至此，此步骤完成。

   ---

   现在可以打开游戏试试效果。

   ### 感谢

   [BV12D421j7mA](https://www.bilibili.com/video/BV12D421j7mA/)
