# 项目中babel的一些操作
* babel src -d lib/ --verbose --copy-files && node script/build.js
* &&  继发执行（即前一个任务成功,才执行下一个任务）


* 编译整个src目录下的文件并输出到lib目录,输出目录可以通过 --out-dir 或 -d  指定。 这不会覆盖lib 目录下的任何其他文件或目录（npx babel src --out-dir lib）
* 复制不需要编译的文件 （npx babel src --out-dir lib --copy-files）