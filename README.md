# hexo-theme-meizi

## 怎么使用

### 安装Hexo

```bash
	npm install hexo-cli -g
```
### 初始化项目
```bash
	hexo init blog
	cd blog
	npm install
	hexo server --debug
```

### 安装Meizi主题
```bash
	cd theme
	git clone https://github.com/imochen/hexo-theme-meizi.git
	mv hexo-theme-meizi meizi
```

### 配置主题

在根目录找到`_config.yml`,将theme改为`meizi`

```javascript
	theme: meizi
```

### 初始化主题

```bash
	hexo new page about
```
打开新创建的`about/index.md`
修改其内容为
```md
	title: "关于我"
	layout: "about"
	---

	<!-- 这里写你的简介 -->
```


```bash
	hexo new page archive
```
打开新创建的`archive/index.md`
修改其内容为，里面无需再追加任何内容
```md
	title: "归档"
	layout: "all-archives"
	---
```


```bash
	hexo new page tags
```
打开新创建的`tags/index.md`
修改其内容为，里面无需再追加任何内容
```md
	title: "标签"
	layout: "tags"
	---
```

### 启动预览

重新启动Hexo
```bash
hexo server --debug
```

## 二次开发

### 安装开发依赖工具

进入主题目录，安装依赖
```bash
	npm install
```

安装完成后启动gulp任务即可

```bash
	gulp watch
```