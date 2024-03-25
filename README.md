# electron-python

### 简介

electron 打包成 mac、win ，调用python 程序

### 技术栈

- electron、
- vue3
- vite
- electron
- python


### 目录结构

~~~

├─┬─┬ extend        扩展的放python程序  
│ │ └── hello
│ │
│ ├─┬ dist         前端build后的文件
│ │ ├── index.html
│ │
│ ├─┬ dist-electron
│ │ ├── main.js
│ │ └── preload.js
│ │
│ ├─┬ electron
│ │ ├── main.js
│ │ └── preload.js
│

~~~


### 使用

打包 python

```sh
PyInstall start.py
```

把打包后的内容放到 ` extend ` 目录

打包 应用程序

```sh
# 打包electron - mac
npm run build-mac
# 打包electron - windows
npm run build-win


```

### 配置

配置 `.env`

```ini
# 配置执行的主py程序

MAIN_VITE_SCRIPT_MAIN = 'start'

# 配置一个 密钥key
MAIN_VITE_SCRIPT_KEY = 'xxxxx'


# 其他自定义环境变量
MAIN_VITE_XXXX = 'xxxxx'

```


### 更新记录

> 2024-03-26
- 实现 electron打包mac、打包win；调用python 脚本



### 交流

- email：343196936@qq.com（加请备注）
- qq：343196936（加请备注）
