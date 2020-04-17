# Fate/Grand Order Android客户端开启60帧的方法
### 注：使用Mumu模拟器，在国服v1.66.0版本测试可行，需要root。
原理修改游戏的SharedPreference文件

文件路径：/data/user/0/com.bilibili.fatego/shared_prefs/com.bilibili.fatego.v2.playerprefs.xml

或/data/data/com.bilibili.fatego/shared_prefs/com.bilibili.fatego.v2.playerprefs.xml

(若模拟器上存在多开FGO，则其他客户端的位置可能在/user/X上，X为非0数字）

在文件中查找int值"OptionHighFPS"，修改为1即可。若没有找到，则直接添加行

&lt;int name="OptionHighFPS" value="1" /&gt;

修改后保存，启动FGO，就可以看到效果了

这样就不用每次都去更新MuMu模拟器了
