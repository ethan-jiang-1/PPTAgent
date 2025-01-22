# 项目结构深度分析

## 核心架构
- `requirements.txt`: 主要依赖清单，包含了机器学习和 NLP 相关的库
  - transformers, FlagEmbedding: 表明项目可能涉及语言模型或嵌入
  - pdf2image, PyPDF2, python-pptx: 文档处理相关
  - vllm: 大语言模型推理优化

- `.pre-commit-config.yaml`: 代码质量控制
  - black + isort: Python 代码格式化
  - 使用了最新的 black 24.4.0 版本
  - isort 配置与 black 兼容

## 环境管理
- `.env`: 环境变量配置
  - 可能包含 API keys, 模型路径等敏感信息
  - 建议添加到 .gitignore
- `requirements_macos.txt`: macOS 特定依赖
  - 包含 M1/M2 芯片的特定优化包
  - 与主依赖清单分离管理

## 工程特点
1. 模块化设计
   - 环境配置与代码分离
   - 平台特定依赖单独管理
2. 自动化程度高
   - 代码质量自动化
3. 跨平台支持
   - 考虑了 macOS 特殊需求 