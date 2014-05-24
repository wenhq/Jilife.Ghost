# Ghost的定制版
原版说明见[Ghost](https://github.com/TryGhost/Ghost#ghost-)。使用postgre数据库，并考虑更换评论系统。

## 快速使用:

1. `npm install -g grunt-cli`
1. `npm install`
1. `grunt init` (and `grunt prod` if you want to run Ghost in production mode)
1. `npm start`

如果出现错误，一定是网络问题。删除“node_modules”和“bower_components”目录后，重试。

## windows环境下postgre数据库使用

1. pgAdmin 中创建数据库jilifer
1. 将pg_config.exe所在目录放到PATH环境变量中
1. Windows的CMD中`set NODE_ENV=devpg`，或者在powershell中`$env:NODE_ENV="devpg"`
1. `npm start`有必要的话，先`grunt init`再`npm start`