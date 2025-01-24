# 源代码目录说明

## 核心模块
1. `apis.py`: API 调用和执行管理
   - CodeExecutor: 执行代码动作，管理 API 调用历史
   - API_TYPES: 支持的 API 类型（替换图片、删除段落等）
   - 提供了详细的错误反馈机制

2. `presentation.py`: PPT 文档对象模型
   - Presentation: PPT 文档的核心表示
   - SlidePage: 幻灯片页面管理
   - ShapeElement: 形状元素基类
   - 支持多种形状类型：Picture, TextBox, GroupShape 等

3. `pptgen.py`: PPT 生成引擎
   - PPTGen: PPT 生成的抽象基类
   - PPTCrew: 多智能体协作的 PPT 生成实现
   - 支持模板系统和内容生成

4. `llms.py`: 语言模型集成
   - 支持多种 LLM 模型：GPT-4, Qwen, InternVL 等
   - 提供统一的模型调用接口
   - 包含角色系统和历史记录管理

## 工具模块
1. `utils.py`: 通用工具函数
   - 文件操作和路径管理
   - PPT 格式转换
   - 配置管理和错误处理

2. `model_utils.py`: 模型相关工具
   - 文本和图像嵌入
   - 相似度计算
   - PDF 解析和处理

3. `multimodal.py`: 多模态处理
   - ImageLabler: 图像标注和管理
   - 支持图像信息提取和标注

## 实验模块
1. `experiment/`: 实验相关代码
   - ablation.py: 消融实验实现
   - baseline_*.py: 基准测试实现
   - evals.py: 评估系统
   - crawler.py: 数据爬取工具

## 工作流程
1. 文档分析
   - PDF/PPT 解析
   - 内容提取和结构化
   - 图像处理和标注

2. 内容生成
   - 模板选择和适配
   - 内容规划和组织
   - 多模态内容生成

3. 文档合成
   - 幻灯片布局
   - 内容填充和样式调整
   - 质量控制和优化

## 技术特点
1. 模块化设计
   - 清晰的模块划分
   - 高内聚低耦合
   - 易于扩展和维护

2. 多模型协作
   - 支持多种 AI 模型
   - 统一的接口设计
   - 灵活的模型切换

3. 鲁棒性设计
   - 完善的错误处理
   - 重试机制
   - 详细的日志记录 