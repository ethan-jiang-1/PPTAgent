# 提示词管理说明

## 目录内容
- content_induct.txt: 用于内容归纳和总结的提示词模板
- category_split.txt: 用于内容分类和拆分的提示词模板
- caption.txt: 用于生成标题和说明文字的提示词模板
- ppteval_describe_content.txt: 用于评估和描述PPT内容的提示词模板
- ask_category.txt: 用于询问和确认内容类别的提示词模板

## 深度理解
- 这些提示词文件构成了PPT生成过程的核心流程：从内容归纳、分类拆分、到标题生成和内容评估
- 每个提示词模板都针对特定任务进行了优化，确保AI能准确理解和执行相应任务
- 提示词之间相互关联，形成了一个完整的PPT生成工作流：
  1. 首先使用content_induct进行内容提取和归纳
  2. 通过category_split进行内容的分类和结构化
  3. 使用caption生成合适的标题和说明
  4. 通过ppteval_describe_content评估内容质量
  5. 需要时使用ask_category进行类别确认 