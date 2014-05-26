请安装Unity3D 4.0，本SDK在未经修改的Unity3D 3.5及以下版本中无法正常工作。  
1、	在场景(scene)中添加“Countly prefab”。  
2、	在Hierarchy中点击Countly game object。  
3、	在Countly script中设置以下变量：  
Server URL: https:// api.qiku.mobi  
App Key: 由奇酷分配  
App Version：应用版本号。  
  
可选特性及配置  
调试模式(Debug Mode)：可以通过检查Is Debug Mode On变量的值察看是否处于调试模式。  
手动模式(Manual Mode)：如果你想自己控制用户session的开始和结束，请移除Auto Start变量，你可以在任何时候调用Countly.Instance.OnStart()和Countly.Instance.OnStop()。  
数据检查间隔(Data Check Period)：Countly将在这个设置的时间间隔内检查是否有数据等待发往服务器。  
心跳信息间隔(KeepAliveSendPeriod)：Countly会发送心跳信息以计算session时长，默认间隔为30秒。  
失败后睡眠时间(Sleep After Failed Try)：Countly在连接失败后会等待一段时间后再次尝试，等待的时间为失败次数乘以睡眠时间，默认睡眠时间为5秒。  
数据包大小(Package Size For Events)：Countly会一次发送多个事件数据以减少数据传送，可以设置这个值以改变包的大小。  


