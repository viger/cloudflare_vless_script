# cloudflare_vless_script
## 本项目基于bia-pain-bache/BPB-Worker-Panel，在此感谢原作者。

# ！！！请勿滥用(如果因为你的行为导致CF全面封禁的话，那么你就是历史的罪人。), 请轻度使用CF流量，不然很容易超过worker的使用阈值。

### 关于本项目
- 修改了部分关键字，所以请按照本项目中关键字配置
- 添加了github action自动部署功能（一次设置，多次部署）
- 采用了不同的混淆方式
- 修改后台地址为https://yourdomain.com/dash
  
### 需要准备的材料
- Fork本项目
- CF账户一枚
- 自有域名一个(非必须)
- 没了

#### 自动部署
由于CF调整了自动部署规则，导致代码部署后混淆失效。请手动部署。

#### 手动部署
将_worker.js中的代码复制到worker代码中，或上传文件到pages。
然后按如下图方式配置即可;
![图片](https://github.com/user-attachments/assets/b700eaea-512f-488a-9d45-0367301c8787)

