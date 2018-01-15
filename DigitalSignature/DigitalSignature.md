# 数字签名是什么？
[原文链接](http://www.ruanyifeng.com/blog/2011/08/what_is_a_digital_signature.html)
## 数字签名是什么？
1. 
![](http://www.ruanyifeng.com/blogimg/asset/201108/bg2011080901.png)  

鲍勃有两把钥匙，一把是公钥，另一把是私钥。  

2. 
![](http://www.ruanyifeng.com/blogimg/asset/201108/bg2011080902.png)  

鲍勃把公钥送给他的朋友们----帕蒂、道格、苏珊----每人一把。  

3. 
![](http://www.ruanyifeng.com/blogimg/asset/201108/bg2011080903.png)  

苏珊要给鲍勃写一封保密的信。她写完后用鲍勃的公钥加密，就可以达到保密的效果。  

4. 
![](http://www.ruanyifeng.com/blogimg/asset/201108/bg2011080904.png)  

鲍勃收信后，用私钥解密，就看到了信件内容。这里要强调的是，只要鲍勃的私钥不泄露，这封信就是安全的，即使落在别人手里，也无法解密。  

5. 
![](http://www.ruanyifeng.com/blogimg/asset/201108/bg2011080905.png)  

鲍勃给苏珊回信，决定采用"数字签名"。他写完后先用Hash函数，生成信件的摘要（digest）。  

6. 
![](http://www.ruanyifeng.com/blogimg/asset/201108/bg2011080906.png)  

然后，鲍勃使用私钥，对这个摘要加密，生成"数字签名"（signature）。  

