# 1.5.0 (2023-09-5)

### ✔️ refactor

- 重构puretab组件

### 🎫 Feat

- 添加了puretab权限按钮

### 🐞 Bug fixes

- "修正添加人员"的弹窗组件事件的bug
- 修复 `RePureTableBar` 组件初始化时列设置勾选项未根据 `hide` 属性正确初始化

# 以下版本是基于pureadmin的再次开发版本，对组件进行再次封装

# 1.0.0 (2023-09-2)

### ✔️ refactor

- 对puretab组件的再次封装，对edit函数的重构，，添加了"添加人员"的弹窗组件，并且添加了更多的交互和实用功能

### 🎫 Feat

- 重构了puretab编辑函数的重构

### 🐞 Bug fixes

- 修复了puretab部分交互的不合理性
- 修正了两个右键弹出框的矛盾事件

### 🍏 Perf

- 页面切换性能优化，不考虑网络的情况下，页面切换逻辑的速度差不多比之前快 `3-4` 倍 [查看优化详情](https://github.com/pure-admin/vue-pure-admin/pull/600#issuecomment-1586094078)
- 优化标签页操作-路由传参模式用法
- 系统管理中表格均改为自适应内容区高度，需将 `@pureadmin/table` 升级到最新版
- 使用 `vueuse` 的 `useResizeObserver` 函数替换 `v-resize` 自定义指令，从测试后的表现来看性能会更好
- 对未解绑的公共事件，在页面销毁时解绑
