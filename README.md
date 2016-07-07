# AllThatRecorderLite
破解 All That Recorder Lite.apk 方法

=================

应用名称：All That Recorder Lite.apk

应用包名：com.pjw.atrl

备注：此应用限制MP3和OGG录音时间为1分钟

破解方法：

① 首先，反编译 All That Recorder Lite.apk，然后反编译 classes.dex。

② 找到 com/pjw/atrl/S.smali 文件并打开，定位到如下代码：

	# direct methods
	.method static constructor <clinit>()V
    .registers 7

    .prologue
    const/4 v6, 0x5

    const/4 v1, 0x3

    const/4 v5, 0x1   //将 0x1 修改为 0x0

    const/4 v4, 0x2

    const/4 v3, 0x0

    .line 47
    sput-boolean v5, Lcom/pjw/atrl/S;->LITE:Z


按照上述标注修改然后保存。
即可破解1分钟限制！

最后编译，然后安装 All That Recorder Pro.apk 。破解完成！

=================

【特别声明】

👉 不保证上述破解方法永久有效！ 
如果此应用开发者重新修改代码，那上述破解方法就失效！这你必须要清楚明白！

👉 开发者敲字母编写程序代码也不容易，如果你条件(不管是经济还是网络条件)允许，还是请通过 Google Play商店 支付美元购买原版APK应用！以支持开发者的开发工作。

👉 我破解是因为我没有上述那个条件。穷逼无美元的破解者一个。 如果你愿意，请捐赠以支持我的破解工作。

👉 如果你还有问题？请 <a href=https://github.com/APK-Patched/AllThatRecorderLite/issues>在此</a> 提交你的问题。
