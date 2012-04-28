# MacOSX Terminal环境配置

## 安装概要

**相关软件列表**

**iTerm2**

__homebrew__

	/usr/bin/ruby -e "$(/usr/bin/curl -fksSL https://raw.github.com/mxcl/homebrew/master/Library/Contributions/install_homebrew.rb)"
	
	brew update
	brew install wget
	brew install tmux
	brew install ruby
	brew install brew-gem
	brew install imagemagick
	brew install lua
	brew install node
	brew install mysql
	brew install snmp

#### 设置环境变量

	echo "export PATH=/usr/local/Cellar/ruby/1.9.3-p125/bin:$PATH" >> ~/.profile
	. ~/.profile
	
#### 安装MySQL

	brew install mysql
	unset TMPDIR
	mysql_install_db --verbose --user=`whoami` --basedir="$(brew --prefix mysql)" --datadir=/usr/local/var/mysql --tmpdir=/tmp

	mysql.server start

	A "/etc/my.cnf" from another install may interfere with a Homebrew-built

	mkdir -p ~/Library/LaunchAgents
	cp /usr/local/Cellar/mysql/5.5.20/homebrew.mxcl.mysql.plist ~/Library/LaunchAgents/
	launchctl load -w ~/Library/LaunchAgents/homebrew.mxcl.mysql.plist
