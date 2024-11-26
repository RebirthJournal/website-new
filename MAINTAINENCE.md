# 技术文档

## 配置开发环境

这段文档将指导您如何在本地构建和运行网站，供您在本地开发和调试。

网站使用 [Jekyll](https://jekyllrb.com/) 构建。此处默认您使用的是 macOS 系统，并且较为熟悉命令行操作。对于 Windows 系统，请自行查找相关资料。

首先，你需要确保已经安装了 Homebrew，如果没有，请参考 [Homebrew 官网](https://brew.sh/) 安装。

然后，安装 Ruby:

```bash
brew install ruby
```

您还需要手动配置 Ruby 环境变量，将以下内容添加到 `~/.bash_profile` 或 `~/.zshrc` 文件中：

```bash
export PATH="/opt/homebrew/opt/ruby/bin:$PATH"
```

然后，安装 `Jekyll` 和 `Bundler`:

```bash
gem install bundler jekyll
```

将这个仓库克隆到本地并且切换到仓库目录:

```bash
git clone https://github.com/RebirthJournal/website.git
cd website
```

安装依赖:

```bash
bundle install
```

运行网站:

```bash
bundle exec jekyll serve
```

此时网站应该已经在本地运行，打开浏览器访问 `http://localhost:4000` 。

## 部署

网站使用 [GitHub Pages](https://pages.github.com/) 部署。
