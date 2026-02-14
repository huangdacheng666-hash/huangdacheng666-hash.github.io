# Allen Huang 个人简历网站

基于 [hexo-theme-snail](https://github.com/dusign/hexo-theme-snail) 开发的个人简历网站，支持中英文双语。

## 访问地址

- **中文站**: https://huangdacheng666-hash.github.io/
- **英文站**: https://huangdacheng666-hash.github.io/en/

## 管理后台

- **CMS后台**: https://huangdacheng666-hash.github.io/admin/
- 登录后可在线编辑简历内容

## 功能特性

- [x] 中英文双语支持
- [x] 响应式设计
- [x] 在线内容管理 (Decap CMS)
- [x] 自动部署到 GitHub Pages

## 快速开始

### 1. 创建 GitHub 仓库

1. 登录 GitHub
2. 创建新仓库，名称为：`huangdacheng666-hash.github.io`
3. 将本项目所有文件上传到仓库

### 2. 配置 GitHub Pages

1. 进入仓库 Settings
2. 找到 Pages 选项
3. Source 选择 **Deploy from a branch**
4. Branch 选择 **gh-pages**，目录选择 **/(root)**
5. 保存设置

### 3. 启用 Git Gateway (CMS 权限)

1. 进入仓库 Settings
2. 找到 **Developer settings** → **Personal access tokens** → **Tokens (classic)**
3. 生成新 Token，名称随意，权限勾选 `repo`
4. 保存 Token（只显示一次）

或者更简单的方法：
1. 进入仓库 Settings
2. 找到 **Code and automation** → **Actions** → **General**
3. 滚动到底部，Workflow permissions 选择 **Read and write**
4. 保存

### 4. 访问网站

- 主站: `https://huangdacheng666-hash.github.io/`
- CMS后台: `https://huangdacheng666-hash.github.io/admin/`

## 内容管理

### 通过 CMS 后台管理

1. 访问 `/admin` 页面
2. 使用 GitHub 账号登录
3. 可以编辑工作经历、教育背景等内容

### 手动编辑

文件位置：
- 中文内容: `source/_posts/work-experience-cn.md`
- 英文内容: `source/_posts/work-experience-en.md`
- 中文关于: `source/about/index.md`
- 英文关于: `source/en/about/index.md`

## 公司链接

已在简历中添加以下公司链接：

| 公司 | 官网 |
|------|------|
| 昆山丘钛智行致远科技有限公司 | https://www.qtechsmartvision.com/ |
| 深圳市卓驭科技有限公司（大疆车载） | https://www.dji.com/automotive |
| 深圳市商汤科技有限公司 | https://www.sensetime.com |
| 杭州海康威视数字技术股份有限公司 | https://www.hikvision.com |
| 深圳市大疆创新科技有限公司 | https://www.dji.com |

## 添加 CloudFlare 域名

1. 在 CloudFlare 添加域名
2. 将域名的 DNS 解析指向 `huangdacheng666-hash.github.io`
3. 在 GitHub 仓库中添加 CNAME 文件（已配置）

## 项目结构

```
├── _config.yml          # Hexo 主配置
├── package.json         # 依赖配置
├── source/
│   ├── _posts/          # 简历内容
│   │   ├── work-experience-cn.md
│   │   └── work-experience-en.md
│   ├── about/           # 关于页面
│   ├── en/              # 英文页面
│   ├── admin/           # CMS 后台
│   ├── img/             # 图片资源
│   └── css/             # 自定义样式
├── themes/snail/        # 主题文件
└── .github/workflows/   # 自动部署配置
```

## 技术栈

- **静态网站生成器**: Hexo
- **主题**: hexo-theme-snail
- **内容管理**: Decap CMS
- **托管**: GitHub Pages
- **自动部署**: GitHub Actions

## 许可证

基于 Apache-2.0 许可证开源。
