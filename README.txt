SPARDEE Website - GitHub Pages + Namecheap 域名部署指南

1. 创建 GitHub 仓库，例如：spardee-site

2. 上传本文件夹中的所有内容（包括 CNAME 文件）

3. 在 GitHub 仓库中启用 GitHub Pages：
   - Settings > Pages > Source: "Deploy from a branch"
   - Branch: main，点击 Save
   - 填写自定义域名：spardee.com，勾选 "Enforce HTTPS"

4. 登录 Namecheap：
   - 进入 "Domain List" → 点击你的域名 → "Advanced DNS"
   - 添加 4 条 A 记录：

     Type: A | Host: @ | Value: 185.199.108.153 | TTL: Automatic
     Type: A | Host: @ | Value: 185.199.109.153 | TTL: Automatic
     Type: A | Host: @ | Value: 185.199.110.153 | TTL: Automatic
     Type: A | Host: @ | Value: 185.199.111.153 | TTL: Automatic

   - （可选）添加 CNAME：Type: CNAME | Host: www | Value: your-github-username.github.io

5. 等待 DNS 生效后，访问 spardee.com 即可看到你的网站！
