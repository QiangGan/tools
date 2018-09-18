=======================================

\#		vim's command					\#

=======================================

* In file ~/.vimrc set `set number`  set line number
*  `gg` go to first line
* `shift +g` go to last line
* `/+[search item]` search content
* `ngg` go to nth line
* `0` go to the begin of line
* `$` go to the end of line
* `dd` delete the current line
* `d$` delete the content from current cursor to line end
* `dw` delete the content from current cursor to word end

========================================

\#		Export Command				\#

========================================

* `export PATH=xxx:$PATH` set environment variable PATH
* `export HOMEBREW_NO_AUTO_UPDATE=true` close brew automatic update

========================================

\#		Location Command				\#

=========================================

* `which [command]` check whether a command exists

* `whereis [filename] `	check whether a file exist
  * -s source file
  * -b binary file
  * -m manual file

============================================

\# 		System info Command			\#	

============================================

* `df -lh` view disk 
* `free -h` view memory
* `cat /proc/cpuinfo` view cpu
* `cat /etc/centos-release` view system version or `cat /etc/redhat-release`

=============================================

\#             Small Script 						\# 

=============================================

```shell
# cr.sh :CR Script
result=$(git stash)
git pull --rebase origin mainline
cr $@
[[ $result =~ "No local changes to save" ]] || git stash pop
```

==============================================

\# 		SSH Command					\#

==============================================

