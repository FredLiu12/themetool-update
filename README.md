## 使用方法

```shell
# 安装依赖
npm i

# 如果electron依赖下载失败，可以设置镜像为淘宝源
npm config set registry https://registry.npmmirror.com/
npm config set ELECTRON_MIRROR https://npmmirror.com/mirrors/electron/

# 运行
npm run electron:serve
# 打包
npm run electron:build
```
注意存放项目路径不能包括中文

macos如果打包出现错误`Error: Exit code: ENOENT. spawn /usr/bin/python ENOENT`
请按以下配置：
修改node_modules/dmg-builder/out/dmg.js，搜索python，修改/usr/bin/python为你的python绝对路径（python2哦）
例如`/Library/Frameworks/Python.framework/Versions/2.7/Resources/Python.app/Contents/MacOS/Python`
