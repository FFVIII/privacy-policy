# 新 App 隐私政策 + 支持页 — 提示词模板

以后做新 App 时，把下面这段发给 Claude，填好 App 信息即可。
流程完全对齐 `shopping-list/`。

---

```
帮我为一个新 App 建隐私政策 + 支持页，放到 privacy-policy 仓库里，
完全按照 shopping-list 那套流程和风格来做。

【App 信息】(我填)
- App 名称(英文):
- App 名称(中文):
- 文件夹 slug(小写连字符，如 shopping-list):
- 一句话简介:
- 数据是否只存本地、不上传?(是 / 否——若否说明上传了什么):
- 用到的权限(如 通知/相机/照片/位置/麦克风，没有就写「无」):
- 是否用了第三方服务(分析/广告/崩溃统计，没有写「无」):
- 支持页想放的 FAQ 要点(列几条即可，可留空让你帮我想):

【要求】
1. 隐私政策和支持页都要中英双语，沿用 shopping-list 的 HTML 模板和样式。
2. 内容要贴合上面填的实际功能和权限，别照抄无关条款。
3. 把新 App 加到 index.html 首页列表。
4. commit 并 push 到远程(务必 push，别只在本地提交)。
5. 推送后 poll 验证 privacy 和 support 两个网址都返回 200 再告诉我完成。
6. 最后给我这两个网址，标好哪个填 Privacy Policy URL、哪个填 Support URL。
```

---

## 完成后填进 App Store Connect

- **Privacy Policy URL**: `https://ffviii.github.io/privacy-policy/<slug>/`
- **Support URL**: `https://ffviii.github.io/privacy-policy/<slug>/support/`
