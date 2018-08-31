1.使用步骤
   a:首先下载下来然后把你的apk放入到项目中的PythonTool中的目录下,
   b:然后打开终端cd到项目中.把.py文件拉进去直接按下Enter(确定键)就OK啦.你就可以看到很多渠道包
2.如果查看是否渠道文件打成功了呢
   a:如果androidstudio开着的话,直接把apk拖到as里面你就可以看到他把apk文件以zip的形式展示出来了
   b:进入到META-INF文件中 会发现有一个cztchannel_chuizi的文本名字.就说明这一步操作没问题啦
3.如果在as项目中获取渠道呢
   a:项目中有一个JavaUtil文件夹,打开之后就会发现又一个java文件
   b:把java文件放入到你的项目中 作为一个工具类
   c:ChannelUtil.getChannel(Context); 通过这段代码获取渠道,一般都是在Application中获取,然后给umeng等统计平台init过去渠道.
   d:为了方便统计是不是获取到了渠道,如果没有获取渠道是execption渠道.不然的话是default渠道.统计的时候会蒙蔽
