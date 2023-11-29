# 快速开始

#### 安装组件库
```bash
npm i sx-ui2
```

#### 引用组件库
> 在manin.js 中引用组件库

```javascript
// 全部引入
import 'sx-ui2/dist/css/index.css';
import MUI from 'sx-ui2';
Vue.use(MUI);

// 按需引入
import 'sx-ui2/dist/css/demo.css';
import { Demo } from 'sx-ui2';
Vue.use(Demo);
```