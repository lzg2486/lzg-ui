# 快速开始

#### 安装组件库

```bash
npm i lzg-ui
```

#### 引用组件库
> 在main.js中引用组件库

```javascript
// 全部引入
import 'lzg-ui/dist/css/index.css'
import LUI from 'lzg-ui'
Vue.use(LUI)

// 按需引用
import 'lzg-ui/dist/css/demo.css'
import { Demo } from 'lzg-ui'
Vue.use(Demo)
```