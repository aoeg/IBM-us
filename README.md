fork [https://github.com/CCChieh/IBMYes](https://github.com/CCChieh/IBMYes)  


# fork修改内容:
* `Secrets` 加入 `V2_ID`, `V2_PATH`, `ALTER_ID`,  
  对应`vmess id`, `ws path`, `alterId`
* 使用actions, 每周自动更新`v2ray`, 部署到 `IBM Cloud Foundray`.


# 配置流程



* 点击 `Secrets` 建立以下几个`secret`, 不修改默认值的可以不建:  
    |  |  |
    | ---- | ---- |
    | IBM_ACCOUNT  | IBM Cloud的登录邮箱和密码, 一行邮箱, 一行密码.   |
    | IBM_APP_NAME | IBM应用的名称.|
    | IBM_MEMORY   | IBM应用内存大小, 默认值`128M`.|
    | V2_ID        | vmess id, 默认值`d007eab8-ac2a-4a7f-287a-f0d50ef08680`.|
    | V2_PATH      | ws path, 默认值`path`.|
    | ALTER_ID     | alterId, 默认值`0`.|
    | VLESS_EN     | 是否使用`vless`, 默认值`true`.|
* 点击项目 `Actions`, 点击`IBM Cloud Deploy`, 点击`Run workflow`, 后续每周会自动部署一次(IBM 10天不用会停).
* 如果需要其他配置, 可以编辑自己仓库的`config/config.json`文件.

