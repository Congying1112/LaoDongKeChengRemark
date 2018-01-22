# truffle课程环境配置(Mac版)
### 环境安装
```
// 安装nvm
$ curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.8/install.sh | bash
// 选node版本
$ nvm install v6
// 配淘宝镜像（国内同学）,之后用cnpm代替npm
$ npm install -g cnpm --registry=https://registry.npm.taobao.org
// 安装truffle
$ cnpm install -g truffle
// 安装GANACHE（以太坊客户端）
$ cnpm install -g ganache-cli
```

### 示例环境
```
$ mkdir ${PROJECT_DIR}
$ cd ${PROJECT_DIR}
$ truffle init
$ truffle unbox MetaCoin
```
参考 http://truffleframework.com/docs/advanced/configuration 配置truffle.js，比如：
```
module.exports = {
  networks: {
  	development: {
  		host: "localhost",
  		port: 8545,
  		network_id: "*"
  	}
  }
};
```

### 运行ganache客户端
```
$ ganache-cli
```

### 然后就可以愉快地玩耍了
