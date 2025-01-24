# PPTAgent UI 说明

## 目录结构
pptagent_ui/
├── src/
│   ├── components/
│   │   ├── Generate.vue    # PPT生成组件
│   │   └── Upload.vue      # 文件上传组件
│   │   
│   ├── router/
│   │   └── index.js        # 路由配置
│   ├── App.vue             # 主应用组件
│   └── main.js             # 应用入口
├── backend.py              # Python后端服务
└── vue.config.js           # Vue项目配置

## 深度理解
- 前端采用 Vue.js 框架，实现了一个完整的PPT生成工具：
  1. Upload.vue 处理文件上传，支持多种格式的文档输入
  2. Generate.vue 负责PPT生成流程，与后端API交互
  3. 路由系统实现了页面导航和状态管理
  
- backend.py 提供后端服务：
  1. 处理文件上传和存储
  2. 调用AI模型进行内容处理
  3. 生成PPT并返回结果
  
- 整体架构采用前后端分离：
  1. 前端负责用户交互和数据展示
  2. 后端负责业务逻辑和AI处理
  3. 通过API实现前后端通信 