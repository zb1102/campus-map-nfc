# 校园地图 NFC 页面

这是给 NT3H2111 NFC 标签使用的极简静态网页。手机碰 NFC 后打开这个网页，页面只显示校园地图图片。

## 使用方法

1. 把校园地图图片放到 `assets` 文件夹。
2. 文件名改成下面任意一个：
   - `campus-map.png`
   - `campus-map.jpg`
   - `campus-map.jpeg`
   - `campus-map.webp`
3. 打开 `index.html` 本地预览。
4. 部署整个 `campus-map-nfc` 文件夹到支持 HTTPS 的服务器。
5. 把部署后的 HTTPS 地址写入 NT3H2111 的 NDEF URI。

示例 NFC 写入内容：

```text
https://your-domain.com/campus-map-nfc/
```

注意：iPhone 通常会先弹出 NFC 提示，点击后才打开页面，这是系统限制。
