# Shuang (Twist) Song 的博客

欢迎访问我的[个人博客主页](https://songshgeo.com)！

![个人banner2](https://songshgeo-picgo-1302043007.cos.ap-beijing.myqcloud.com/uPic/%E4%B8%AA%E4%BA%BAbanner2.png)

## 关于

这是一个基于 Hexo 框架搭建的个人博客，使用 matery 主题，专注于地理学、旅行、阅读和个人思考的分享。

- **标题**: Twist
- **作者**: Shuang (Twist) Song
- **简介**: A geographer who also travels.
- **网站**: https://songshgeo.com

## 技术栈

- **框架**: [Hexo](https://hexo.io/) 7.3.0
- **主题**: [matery](https://github.com/blinkfox/hexo-theme-matery)
- **语言**: Node.js / Markdown
- **特性**: 
  - Material Design 风格
  - 响应式设计
  - 支持 RSS 订阅
  - 中文链接转拼音（SEO 优化）
  - 文章字数统计
  - 代码高亮

## 快速开始

### 环境要求

- Node.js 14.0+
- npm 或 yarn

### 安装依赖

```bash
npm install
```

### 本地开发

```bash
# 启动本地服务器
npm run server

# 访问 http://localhost:4000
```

### 构建部署

```bash
# 清理缓存
npm run clean

# 生成静态文件
npm run build

# 部署到服务器
npm run deploy
```

## 项目结构

```
.
├── source/              # 源文件目录
│   ├── _posts/         # 博客文章（Markdown 格式）
│   │   ├── 月光/       # 随笔散文
│   │   ├── 年轮/       # 回忆录
│   │   ├── 日渐/       # 日常记录
│   │   └── Album/      # 专题集锦
│   ├── 404.md          # 404 页面
│   ├── about/          # 关于我
│   ├── categories/     # 分类页
│   ├── tags/           # 标签页
│   └── ...
├── themes/matery/      # Matery 主题
├── public/             # 生成的静态网站文件
├── _config.yml         # 博客配置文件
└── package.json        # 项目依赖配置
```

## 文章分类

博客文章主要分为以下几个类别：

- **月光**: 随笔散文、文学创作
- **年轮**: 生活回忆、成长感悟
- **日渐**: 日常记录、效率工具
- **Album**: 专题系列（纪录片推荐、江南行、新年随笔等）

## 开发与维护

### 常用命令

```bash
# 创建新文章
hexo new post "文章标题"

# 创建新页面
hexo new page "页面名称"

# 清理缓存并重新生成
hexo clean && hexo generate

# 本地预览
hexo server
```

### 插件

项目使用了以下 Hexo 插件：

- `hexo-generator-feed`: RSS 订阅生成
- `hexo-generator-search`: 全文搜索
- `hexo-permalink-pinyin`: 中文链接转拼音
- `hexo-wordcount`: 文章字数统计

## 主题定制

主题配置位于 `themes/matery/_config.yml`，可以自定义：

- 导航菜单
- 个人信息
- 社交链接
- 评论系统
- Banner 图片
- 主题颜色

更多配置说明请参考 [Matery 主题文档](https://github.com/blinkfox/hexo-theme-matery/blob/README_CN.md)。

## License

本项目采用 MIT 许可证。博客文章内容版权归作者所有。