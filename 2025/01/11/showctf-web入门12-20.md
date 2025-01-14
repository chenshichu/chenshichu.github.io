---
title: showctf web入门12~20
date: 2025-01-14 16:09:55
tags:
---

    **web 12:**

![28ee1e70-4f61-4db0-9fd3-0021d8a1fe6e](file:///C:/Users/34640/Pictures/Typedown/28ee1e70-4f61-4db0-9fd3-0021d8a1fe6e.png)

1. 进入网页后先查看源代码发现什么也没有  再抓包发现也是一无所获

2. 用虚拟机kali 命令dirsearch 网页地址 -e*扫描网页    发现robots.txt

![b3658f26-23f4-4cee-aa30-4fd18a7dec5a](file:///C:/Users/34640/Pictures/Typedown/b3658f26-23f4-4cee-aa30-4fd18a7dec5a.png)

robots.txt: 一种协议(robots协议 也称爬虫协议)  作用:显示可访问的页面

3. 进入admin页面出现了登录界面

![d7e382b0-b651-4aac-bcea-0e28e6636a7a](file:///C:/Users/34640/Pictures/Typedown/d7e382b0-b651-4aac-bcea-0e28e6636a7a.png)

4. 猜测账号是:damin

5. 在看了别人写的wp发现密码在刚开始页面的最<u><span><font face="宋体">下面</font>372619038</span></u>

![4353c11f-22ac-4ce4-abe2-b8f4792cdc54](file:///C:/Users/34640/Pictures/Typedown/4353c11f-22ac-4ce4-abe2-b8f4792cdc54.png)

6. 输入账号密码后得到flag







    **web 13:**

![52c15395-4991-423d-9d29-2bcbd6ea37bb](file:///C:/Users/34640/Pictures/Typedown/52c15395-4991-423d-9d29-2bcbd6ea37bb.png)

1. 对网页进行一系列操作(如:查看页面源代码、用dirsearch命令等)

2. 发现一无所获

3. 发现题目给出提示

4. ![3ab6303c-4073-4ef8-9404-d04deb6c7006](file:///C:/Users/34640/Pictures/Typedown/3ab6303c-4073-4ef8-9404-d04deb6c7006.png)

5. 回到网页进行检查在网页的最下放发现document(译:文件)并且可以点击

6. 进入后发现

![aa6b54e9-a9e8-41b6-8105-2979eaf9d4f2](file:///C:/Users/34640/Pictures/Typedown/aa6b54e9-a9e8-41b6-8105-2979eaf9d4f2.png)

7. 直接点击给出的后台地址会发现错误    需要把you-domain改为你的网页地址

8. ![847f1dad-decd-4f3f-84dc-3630fbc1df51](file:///C:/Users/34640/Pictures/Typedown/847f1dad-decd-4f3f-84dc-3630fbc1df51.png)

9. 输入账号和密码后等到flag

10.![ca68595a-5380-49c2-8322-90041a5429ab](file:///C:/Users/34640/Pictures/Typedown/ca68595a-5380-49c2-8322-90041a5429ab.png)





    **Web 14:**

 ![4a31cf71-44ec-44b0-bb28-4d5df65e13db](file:///C:/Users/34640/Pictures/Typedown/4a31cf71-44ec-44b0-bb28-4d5df65e13db.png)

1. 题目给出提示直接访问/editor

2. 进入![bceb53a6-71cb-45e6-96ad-00a84b5c8f61](file:///C:/Users/34640/Pictures/Typedown/bceb53a6-71cb-45e6-96ad-00a84b5c8f61.png)

3. 不管输入什么都会是404页面

4. 然后下意识就去上传一句话木马结果:

5. ![4dcba1f1-eed7-4651-90b7-81e874daefd3](file:///C:/Users/34640/Pictures/Typedown/4dcba1f1-eed7-4651-90b7-81e874daefd3.png)

6. 之后,在上传图片的网络图片中发现网页根目录

7. ![a8b58ac9-3036-4ca7-bbf1-59289bb5d4b3](file:///C:/Users/34640/Pictures/Typedown/a8b58ac9-3036-4ca7-bbf1-59289bb5d4b3.png)

![75245b41-c4f5-49f6-a31f-da8c49ba66fc](file:///C:/Users/34640/Pictures/Typedown/75245b41-c4f5-49f6-a31f-da8c49ba66fc.png)

8. 最后发现var/www/html/nothinghere/fl000g.txt

9. 访问   网站地址/nothinghere/fl000g.txt   得到flag





    **Web 15:**

 ![22af93e6-b5ba-43d3-81ce-a55fecc3aa7c](file:///C:/Users/34640/Pictures/Typedown/22af93e6-b5ba-43d3-81ce-a55fecc3aa7c.png)

1. 先对网页进行操作   在用dirsearch命令扫描后得到

![47b308f3-edf3-49b1-956a-39c63eb1dde3](file:///C:/Users/34640/Pictures/Typedown/47b308f3-edf3-49b1-956a-39c63eb1dde3.png)

2. 访问到admin时发现进入到  后台登录系统

![f01608e2-29b4-4b35-8694-3e7d980eb7a6](file:///C:/Users/34640/Pictures/Typedown/f01608e2-29b4-4b35-8694-3e7d980eb7a6.png)

3. 在查遍整个网页后就发现一个邮件  把邮件号当作密码输入错误  在忘记密码中输入邮件号依然错误

4. 因为忘记密码要输入地点  使用在qq中查找  但我没查到不知道为什么   网上看攻略是查到了

5. ![13db0d12-d8a7-40de-9f90-fe8f99c0120f](file:///C:/Users/34640/Pictures/Typedown/13db0d12-d8a7-40de-9f90-fe8f99c0120f.png)![1d924f89-2685-417f-aaba-a4fbcf37a36e](file:///C:/Users/34640/Pictures/Typedown/1d924f89-2685-417f-aaba-a4fbcf37a36e.png)

6. 在忘记密码中输入  西安  给出新密码

7. 在登录中账号:admin  密码:给出的

8. 得到flag:![9bd36bfb-5720-4c90-866b-ff7fe70756be](file:///C:/Users/34640/Pictures/Typedown/9bd36bfb-5720-4c90-866b-ff7fe70756be.png)

    

 

   **Web 16:**

 ![3450a1d5-e92e-4fb6-844f-95926cfd0b66](file:///C:/Users/34640/Pictures/Typedown/3450a1d5-e92e-4fb6-844f-95926cfd0b66.png)

1. 题目给出提示测试探针

2. 探针:![5673143a-c04c-48cd-aba1-dee31e49008a](file:///C:/Users/34640/Pictures/Typedown/5673143a-c04c-48cd-aba1-dee31e49008a.png)

3. 在访问url加入后缀后

![e3bbda53-daff-48de-92c8-dc1c6c39320f](file:///C:/Users/34640/Pictures/Typedown/e3bbda53-daff-48de-92c8-dc1c6c39320f.png)

4. 点击phpinfo进入

![1863743a-8e19-418e-8544-14d017e0c991](file:///C:/Users/34640/Pictures/Typedown/1863743a-8e19-418e-8544-14d017e0c991.png)

5. 搜索flag

6. 找到flag





    **Web 17:**

 ![fa44361f-c81a-449a-a9d9-a3d5e548096d](file:///C:/Users/34640/Pictures/Typedown/fa44361f-c81a-449a-a9d9-a3d5e548096d.png)

1. 提示说会有文件泄露  这种情况一般直接用命令dirsearch扫描网页

2. 扫描结果

3. ![1f09c509-d673-4910-87d5-6665a6acce6d](file:///C:/Users/34640/Pictures/Typedown/1f09c509-d673-4910-87d5-6665a6acce6d.png)

4. 直接访问网页/backup.sql

5. 然后就下载

![f976a584-c0b0-41bf-bfdb-ed98a4f5358d](file:///C:/Users/34640/Pictures/Typedown/f976a584-c0b0-41bf-bfdb-ed98a4f5358d.png)

6. 进入直接发现flag

 ![e5f134fe-ed32-4876-a8c9-47ff3009c533](file:///C:/Users/34640/Pictures/Typedown/e5f134fe-ed32-4876-a8c9-47ff3009c533.png)





   ** Web 18:**

 ![1f6f4ace-fb24-480a-a1ff-abd12a8d3f04](file:///C:/Users/34640/Pictures/Typedown/1f6f4ace-fb24-480a-a1ff-abd12a8d3f04.png)

1.进入后发现是个小游戏 我觉得一般人都不能通过玩获得flag

2.按f12在调试器的js文件中找到变量score和条件>100

3.直接在控制台输入score=200 在游戏开始时按Enter

 ![e02bd913-28f1-4f4b-89f1-af15d34eac8a](file:///C:/Users/34640/Pictures/Typedown/e02bd913-28f1-4f4b-89f1-af15d34eac8a.png)

4. 幺幺零点皮爱吃皮=110.php

5. 访问网站/110.php 得到flag

6. ![7e68c598-a0b5-44bc-a6bf-137efcb1646d](file:///C:/Users/34640/Pictures/Typedown/7e68c598-a0b5-44bc-a6bf-137efcb1646d.png)

        

**Web 19:**

 ![90d074ea-885a-49bf-8811-7a313982c978](file:///C:/Users/34640/Pictures/Typedown/90d074ea-885a-49bf-8811-7a313982c978.png)

1. 打开网页源代码

2. ![10a0f3eb-434d-48fd-9e82-39a8ee07bb83](file:///C:/Users/34640/Pictures/Typedown/10a0f3eb-434d-48fd-9e82-39a8ee07bb83.png)

3. 根据给出提示直接在f12的hackbar的post中输入

4. ![ae38d148-89b1-40d9-a9be-c97b5f7ff489](file:///C:/Users/34640/Pictures/Typedown/ae38d148-89b1-40d9-a9be-c97b5f7ff489.png)

5. 直接得到flag

6. ![3f5b95a1-73c8-4496-ba28-61e47a8b580b](file:///C:/Users/34640/Pictures/Typedown/3f5b95a1-73c8-4496-ba28-61e47a8b580b.png)

    



**Web 20:**

 ![b7ad222c-89ae-44d2-80e3-48e5e80255e6](file:///C:/Users/34640/Pictures/Typedown/b7ad222c-89ae-44d2-80e3-48e5e80255e6.png)

1. 直接用dirsearch扫描网页  扫描结果为

![7c947d07-3038-47bd-8bf3-bdec9e44e37b](file:///C:/Users/34640/Pictures/Typedown/7c947d07-3038-47bd-8bf3-bdec9e44e37b.png)

2. 接着用命令dirsearch扫描网页/db  得到

![306e349c-c6b3-46f2-9aa3-a75e7fe3bf70](file:///C:/Users/34640/Pictures/Typedown/306e349c-c6b3-46f2-9aa3-a75e7fe3bf70.png)

3. 直接访问下载文件在直接查找flag

![b9d7b1e7-ca50-4b90-b209-0a89b053cbc6](file:///C:/Users/34640/Pictures/Typedown/b9d7b1e7-ca50-4b90-b209-0a89b053cbc6.png)


