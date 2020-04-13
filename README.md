## zeit-UpsGo

UpsGo是一个基于 Go+Vue 开发的又拍云对象存储服务管理应用。

该项目用于直接以函数服务部署UpsGo项目而无需任何其他操作。

使用前请克隆或分叉该项目, 修改`api/main.go`文件下的第12行

```go
// conf 是又拍云配置项
var conf = &Ups{
	Bucket:   "", //Bucket名称
	Operator: "", //被授权的操作员名称
	Password: "", //被授权的操作元密码
	Domain:   "", //加速域名
}
```

稍候你只需要注册 [zeit.co](https://zeit.co) 即可使用now命令或者通过github部署项目。

## 部署

1. `Fork` 项目
2. 克隆项目到本地机器 `git clone URL_OF_FORKED_REPO_HERE`
3. 通过 `now` CLI 直接部署项目 (如果你没有该命令, 运行 `npm install -g now` 安装)
4. 若不希望使用 `now` CLI部署, 请通过zeit面板从你的github项目导入Fork的项目

单击按钮直接部署(由于配置信息未填写, 部署或将无法工作).

[![Deploy to now](https://deploy.now.sh/static/button.svg)](https://zeit.co/new/project?template=xuthus5/zeit-upsgo)