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