# 环境配置说明

## 文件说明
- `.env`: 环境变量配置文件
  - 包含敏感信息，如 API keys
  - 建议添加到 .gitignore
- `requirements_macos.txt`: macOS 特定依赖
  - 包含 M1/M2 芯片的特定优化包
  - 与主依赖清单分离管理

## 使用建议
1. 不要将 .env 文件提交到版本控制
2. 使用环境变量管理敏感信息
3. 保持 requirements_macos.txt 与主依赖清单同步 