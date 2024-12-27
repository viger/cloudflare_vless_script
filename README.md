# cloudflare_vless_script
## 本项目基于bia-pain-bache/BPB-Worker-Panel，在此感谢原作者。

###关于本项目
- 修改了部分关键字，所以请按照本项目中关键字配置
- 添加了github action自动部署功能（一次设置，多次部署）！！！请勿滥用(如果因为你的行为导致CF全面封禁的话，那么你就是历史的罪人。)
- 采用了不同的混淆方式
  
### 需要准备的材料
- Fork本项目
- CF账户一枚
- 自有域名一个(非必须)
- 没了

#### 自动部署
- 获取CF_API_TOKEN
  - 在CF后台打开workers 和 pages页面，在页面最右侧栏，找到“管理API令牌”，点进去
    ![图片](https://github.com/user-attachments/assets/cfa5b9eb-f638-4364-bd88-f964fd8046e9)
  - 创建令牌
    点击“创建令牌”，进入创建令牌环节;
    <img width="800" alt="{3801E8E0-76DE-4151-95F2-BE19629C0EE3}" src="https://github.com/user-attachments/assets/a220a797-c689-44ee-bf4c-b205ec35c79d" />
    选择"编辑 Cloudflare Workers"模板创建令牌,
    <img width="790" alt="{EFDF4F09-BF26-4875-A796-92BC24ACF9FA}" src="https://github.com/user-attachments/assets/6938658a-bc02-4c82-b7f4-1c06bae87184" />
    继续按照如下设置
    ![图片](https://github.com/user-attachments/assets/9b27cb45-403a-4972-9e53-8e3d4afb65c5)
    确认创建
    ![图片](https://github.com/user-attachments/assets/b7b441e4-8585-45f5-b710-a20ae115c4f0)
    你会得到一串由数字字母组成的字符串，请将它复制到文本记录器中保留备用
    ![图片](https://github.com/user-attachments/assets/b6aa054e-4592-4e6c-9afc-d761a77377ce)

   - 获取KV空间ID
     在存储与数据库中找到KV页，复制你想要存储的KV空间的ID到文本记录器中备用(没有的创建一个)
     ![图片](https://github.com/user-attachments/assets/0752bead-5498-413d-99ca-2c50b46bb523)

   - 

#### 手动部署
将_worker.js中的代码复制到worker代码中，或上传文件到pages。
然后按如下图方式配置即可;
![图片](https://github.com/user-attachments/assets/6a5c906e-79fa-401d-8015-5bcf908b35e3)
