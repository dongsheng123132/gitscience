# gitscience.net

GitScience 品牌门户页 —— **论文过时了，实验上 GitHub**。

AI 时代的开源科研基础设施。把科学从「写论文」变成「提交实验」。
旗下三条线:科研虾 SciClaw(找 Gap)、论文体检 PaperGuard(查)、实验 Fork(验证)。

## 技术

纯静态单文件:`index.html`(内联 CSS / JS,无构建步骤,无第三方依赖)。
字体走 Google Fonts:Instrument Serif × IBM Plex Mono × Noto Serif/Sans SC。

## 本地预览

直接双击 `index.html`,或起个静态服务器:

```bash
python -m http.server 8080   # 然后开 http://localhost:8080
```

## 部署到 Vercel(域名 gitscience.net)

```bash
# 方式一:CLI
npm i -g vercel
vercel --prod              # 首次会让你登录 + 关联项目

# 方式二:推到 GitHub 后在 vercel.com 导入仓库,Framework 选 "Other"(纯静态)
# 然后在 Vercel 项目 → Settings → Domains 绑定 gitscience.net(按提示改 DNS)
```

`vercel.json` 已配好 `cleanUrls` + 基础安全响应头。

## 待办 / 占位

- `mailto:hi@gitscience.net` 是占位邮箱,需在域名邮箱服务里开通,或换成你的真实联系方式。
- 科研虾(paper-vault)目前是私有库,页面上标注「内测中」,未挂公开链接;开源后再补。
- OG 预览图(`og:image`)暂未配,可后续加一张 1200×630 的分享图。

## 内容口径(重要)

页面只呈现愿景 + 已开源的 PaperGuard 真实链接。**未夸大**任何高校/政府/基金合作,
对标项目(Sakana / AlphaFold / Self-Driving Lab 等)仅作行业方向参照,footer 已声明无隶属关系。
