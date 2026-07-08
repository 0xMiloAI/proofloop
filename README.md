# ProofLoop

ProofLoop 是一个静态落地页项目，灵感来自 Product Hunt 上的 Badge 项目方向：用同事评价和结构化信号生成可分享的职业信誉档案。

这个版本已经换了名字、文案和布局，没有使用原项目品牌素材。

## 本地预览

直接双击 `index.html` 就能打开。

也可以在这个目录启动一个简单服务器：

```powershell
python -m http.server 5173
```

然后打开：

```text
http://localhost:5173
```

## 部署到 Vercel

1. 新建一个 GitHub 仓库。
2. 把 `outputs/proofloop` 目录里的文件上传到仓库根目录。
3. 打开 [Vercel](https://vercel.com)，选择 `Add New Project`。
4. 导入这个 GitHub 仓库。
5. Framework Preset 选择 `Other`。
6. Build Command 留空。
7. Output Directory 留空或填 `.`。
8. 点击 `Deploy`。

## 部署到 Netlify

1. 打开 [Netlify](https://www.netlify.com)。
2. 选择 `Add new site`。
3. 如果用 GitHub，导入仓库；如果不用 GitHub，可以直接拖拽整个 `proofloop` 文件夹。
4. Build command 留空。
5. Publish directory 填 `.`。
6. 点击发布。

## 部署到 Cloudflare Pages

1. 打开 [Cloudflare Pages](https://pages.cloudflare.com)。
2. 选择 `Create a project`。
3. 连接 GitHub 仓库。
4. Framework preset 选择 `None`。
5. Build command 留空。
6. Build output directory 填 `/` 或 `.`。
7. 点击部署。

## 部署到 GitHub Pages

1. 把 `index.html` 放到 GitHub 仓库根目录。
2. 进入仓库 `Settings`。
3. 打开 `Pages`。
4. Source 选择 `Deploy from a branch`。
5. Branch 选择 `main`，目录选择 `/root`。
6. 保存后等待 GitHub 生成访问链接。

## 后续可改

- 把 `ProofLoop` 改成你的真实产品名。
- 替换首页表单逻辑，接入 Tally、Typeform、Airtable、Supabase 或自己的后端。
- 增加真实用户案例、价格页、登录入口和隐私政策。
