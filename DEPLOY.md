# 校园全能提醒小助手 - 部署指南

## 🚀 快速开始

### 方式一：直接使用（单机版）

直接双击 `widget1.html` 在浏览器打开即可使用。

**注意**：单机版数据存在浏览器本地，换设备或清缓存会丢失。

---

### 方式二：GitHub Pages（推荐，免费永久）

#### 步骤1：创建GitHub仓库

1. 登录 [GitHub](https://github.com)
2. 点击右上角 **+** → **New repository**
3. 仓库名称填 `campus-reminder`
4. 选择 **Public**（公开）
5. 点击 **Create repository**

#### 步骤2：上传文件

在仓库页面，点击 **uploading an existing file**，把以下3个文件拖进去：
- `widget1.html`
- `widget2.html`
- `widget3.html`

点击 **Commit changes**。

#### 步骤3：开启GitHub Pages

1. 进入仓库 → **Settings**（设置）
2. 左侧菜单找到 **Pages**
3. Source 下选择 `Deploy from a branch`
4. Branch 选择 `main`，文件夹选 `/ (root)`
5. 点击 **Save**

#### 步骤4：获取访问链接

等待约2分钟，页面顶部会显示：
```
Your site is live at https://你的用户名.github.io/campus-reminder/
```

分享这个链接给同学即可！

---

### 方式三：本地服务器（学校内网共享）

如果只是宿舍/班级内部使用，可以：

1. 把文件放到局域网一台电脑上
2. 在该电脑安装简单服务器：
   ```bash
   # Python方式（推荐）
   python -m http.server 8080

   # Node.js方式
   npx serve .
   ```
3. 获取该电脑的IP地址（如 `192.168.1.100`）
4. 其他同学访问 `http://192.168.1.100:8080/widget1.html`

---

### 方式四：打包下载（U盘/微信传输）

文件已打包为 `campus-reminder.zip`，解压后直接使用。

---

## ❓ 常见问题

**Q: GitHub访问慢怎么办？**
A: 使用国内镜像或考虑方案三/四

**Q: 多人想共享同一份数据？**
A: 需要添加后端服务（数据库），可联系开发者定制

**Q: 如何更新已发布的内容？**
A: 修改本地HTML文件后，重新上传覆盖即可

---

## 📞 技术支持

如有问题，请联系开发者。
