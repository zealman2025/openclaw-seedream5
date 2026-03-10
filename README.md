# Seedream5

OpenClaw 技能：使用火山引擎豆包 Seedream 5.0 生成或编辑图片。

## 安装

### 方式一：手动安装

```bash
# 克隆或下载到你的 OpenClaw workspace skills 目录
git clone https://github.com/你的用户名/seedream5.git /path/to/workspace/skills/seedream5
```

### 方式二：clawhub 安装（若已注册到 ClawHub）

```bash
clawhub install seedream5
```

## 配置 API Key

本技能需要火山引擎 API Key。任选以下一种方式：

### 方式一：环境变量

```bash
export VOLC_API_KEY="你的API_KEY"
# 或
export ARK_API_KEY="你的API_KEY"
```

### 方式二：openclaw.json（推荐）

编辑 `~/.openclaw/openclaw.json`，在 `skills.entries` 下添加：

```json
{
  "skills": {
    "entries": {
      "seedream5": {
        "apiKey": "你的火山引擎API_KEY"
      }
    }
  }
}
```

### 方式三：ClawPanel / Control UI

在 Skills 页面找到 seedream5，在凭证字段中填写 API Key。

### 获取 API Key

前往 [火山引擎控制台](https://console.volcengine.com/ark/region:ark+cn-beijing/apiKey) 获取。

## 依赖

- [uv](https://docs.astral.sh/uv/)（Python 包管理）
- 脚本会自动安装 `requests`、`pillow`

## 使用示例

详见 [SKILL.md](./SKILL.md)。
