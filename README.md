# [蔚蓝档案抽卡网站](https://ba.bigjackson.top)

一个模拟蔚蓝档案抽卡系统的网站，支持单抽、十连抽、保底机制和统计功能。

## 功能特性

🎮 **抽卡系统**
- 单抽
- 十连抽
- 真实的抽卡概率模拟
- 保底机制 (200抽保底3星，10抽保底2星)

🎯 **角色系统**
- 3星角色 (2.5%概率)
- 2星角色 (18.5%概率)
- 1星角色 (79%概率)
- 包含蔚蓝档案经典角色

## 安装和设置

### 1. 克隆项目
```bash
git clone <repository-url>
cd bluearchieve
```

### 2. 安装依赖
```bash
pip install -r requirements.txt
```

### 3. 创建Telegram机器人
1. 在Telegram中找到 [@BotFather](https://t.me/BotFather)
2. 发送 `/newbot` 命令
3. 按照提示设置机器人名称和用户名
4. 获取机器人Token

### 4. 配置环境变量
1. 复制 `env_example.txt` 为 `.env`
2. 在 `.env` 文件中设置你的机器人Token：
```
TELEGRAM_BOT_TOKEN=your_actual_bot_token_here
```

### 5. 运行机器人
```bash
python bot.py
```

## 使用说明

### 可用命令
- `/start` - 开始使用机器人
- `/gacha` - 单抽 (120钻石)
- `/tenpull` - 十连抽 (1200钻石)
- `/balance` - 查看钻石余额和统计
- `/stats` - 查看详细抽卡统计
- `/menu` - 显示抽卡菜单
- `/help` - 显示帮助信息

### 抽卡概率
- ⭐⭐⭐ 3星角色：2.5%
- ⭐⭐ 2星角色：18.5%
- ⭐ 1星角色：79%

### 保底机制
- 200抽内必定获得3星角色
- 10抽内必定获得2星角色
- 十连抽保证至少有一个2星或以上角色

## 项目结构

```
bluearchieve/
├── bot.py              # 主机器人文件
├── config.py           # 配置文件
├── database.py         # 数据库模块
├── gacha_system.py     # 抽卡系统
├── requirements.txt    # 依赖包
├── env_example.txt     # 环境变量示例
├── README.md          # 项目说明
└── users.json         # 用户数据文件 (运行时生成)
```

## 技术栈

- **Python 3.8+**
- **python-telegram-bot** - Telegram Bot API
- **JSON** - 数据存储
- **随机数生成** - 抽卡概率模拟

## 自定义配置

你可以在 `config.py` 文件中修改：

- 角色列表和概率
- 抽卡价格
- 保底机制设置
- 欢迎消息和帮助信息

## 注意事项

1. 确保你的Python版本为3.8或更高
2. 机器人Token请妥善保管，不要泄露
3. 用户数据存储在本地JSON文件中
4. 初始钻石余额为10,000

## 贡献

欢迎提交Issue和Pull Request来改进这个项目！

## 许可证

MIT License

---

🎮 祝你抽卡欧气满满！✨ 
