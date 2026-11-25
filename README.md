# vrcm-team.github.io

VRCM 分享链接用的域名根站点。

- `.well-known/assetlinks.json`：Android App Links 验证。包名是 `io.github.vrcmteam.vrcm`，指纹是 GitHub 发布签名；如果走 Google Play App Signing，还要加上 Play 的签名指纹。
- `.well-known/apple-app-site-association`：iOS Universal Links 验证，Team ID 是 `YZ73QQ6N2X`。
- `404.html`：分享链接没被系统直接交给 App 时打开。iOS 和 Android 显示“在 VRCM 中打开”（iOS 用 `vrcm://`，Android 用带 vrchat.com 回退地址的 `intent://`）和“前往 VRChat 网站”两个按钮；其他平台原样跳到 vrchat.com。
- `index.html`：根路径跳到介绍页 `/VRCM/`（由 VRCM 仓库发布）。
- `.nojekyll`：防止 Jekyll 忽略 `.well-known` 目录。
