# dalejenny.github.io
## GitHub Actions
[Action](https://docs.github.com/en/actions/quickstarthttps://docs.github.com/en/actions/quickstart)

## Commands
```java
gem install bundler

bundle install --verbose

bundle list

find out jekyll version:
bundle exec jekyll -v

clean up bundle cache:
bundle cache --clear sometimes dosen't make up

navite data resourse:
source 'https://gems.ruby-china.com/'

turn powershell into irb
irb

source 'https://rubygems.org'
gem 'github-pages', group: :jekyll_plugins
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw]
gem 'wdm', '>= 0.1.0' if Gem.win_platform?

gem "webrick", "~> 1.7"

```
当你运行 bundle install 时，Bundler 会检查你的系统中已经安装的 gems。如果 Gemfile 中指定的 gem 已经在你的系统中安装，Bundler 就不会再次下载和安装这个 gem。

这意味着，如果你已经下载并安装了 Gemfile 中的某个 gem，再次运行 bundle install 时，Bundler 会跳过这个 gem。

然而，如果你的 Gemfile 或 Gemfile.lock 发生了变化，或者你运行了 bundle update，Bundler 可能会需要重新下载和安装某些 gem。

```java
source 'https://rubygems.org'
// gem 'github-pages', group: :jekyll_plugins
gem 'jekyll', '~> 4.2.0'
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw]
gem 'wdm', '>= 0.1.0' if Gem.win_platform?
gem "webrick", "~> 1.7"
```

## wdm version dones't match
because ruby 's version is 3.3.4 yet wdm is 0.1.0

bundle update :
bundle update
than bundle install could mind you witch version is rigtht
and the last modify the version of wdm

## run server
在已有的项目中使用 Jekyll，你需要按照以下步骤操作：

首先，确保你已经安装了 Ruby 和 Bundler。你可以在终端中运行 ruby -v 和 bundle -v 来检查它们是否已经安装。如果没有安装，你需要先安装它们。

在你的项目根目录下创建一个名为 Gemfile 的文件（如果还没有的话），并添加以下内容：
```java
source 'https://gems.ruby-china.com/'
gem 'jekyll'
```

这个 Gemfile 告诉 Bundler 你的项目需要 Jekyll gem。

在终端中运行 bundle install 来安装 Jekyll。

运行 bundle exec jekyll new . --force 来在你的项目中创建一个新的 Jekyll 站点。--force 参数告诉 Jekyll 覆盖现有的文件。

运行 bundle exec jekyll serve 来启动 Jekyll 的开发服务器。你现在应该可以在浏览器中访问 http://localhost:4000 来查看你的 Jekyll 站点。

请注意，这些步骤会覆盖你项目中的一些文件，如 index.md 或 Gemfile。在运行这些命令之前，你可能需要备份你的项目。

