# KAISAR NETWORK [去注册 https://zero.kaisar.io](https://zero.kaisar.io/register?ref=uqSUWd326)
## Depoloy TG communicate channel [TG CHANNEL](https://t.co/2f0y7mCn1K)
## Depoloy TWITTER communicate channel [X CHANNEL](https://x.com/mooinchain) 

Your compute, your currency
Transform your compute power into real earnings

![banner](image.png)

# Kaisar Beta Cli Mode

## Features

- Support Multy accounts.
- Support Proxy.

## Requirements

- Node.js 20+
- Dependencies installed via `npm install`

## Files

- **if you already have account you can create file manually**
- `tokens.txt`: Stores access_tokens each line 1 account.
- `id.txt`: Stores Extension IDs each line 1 account.
- `proxy.txt`: stores Proxy url format `http://user:pass@ip:port` each line 1 proxy.
- **if you register using cli, file above auto filled, just fill `email.txt` with your email.**
- `emails.txt`: Store email account 1 line 1 account.

## Usage 
一个账号，项目方禁止开多IP节点挖矿，至于为什么 不清楚

1. Clone the repository:
   ```bash
   git clone https://github.com/amumuku/kaisar-bot.git
   cd kaisar-bot
   ```
2. 安装依赖:
   ```bash
   npm install
   ```
3.下面准备好批量邮箱地址
   ```
    填充到emails.txt
   ```
4. 注册邮件发验证码（新账户），老账户会直接生成token(官方已升级平台，已经失效，走手动注册)
   ```bash
   npm run register（废弃）
   ```
   手动注册后，打开检查窗口，找到请求的令牌token ，复制到token.txt里面
   <img width="703" alt="image" src="https://github.com/user-attachments/assets/81fc4d8a-d730-4c8a-8180-73660168fc30" />

5.验证邮件并confirm
   ```
   检查上面所有的邮箱的验证邮件并confirm,完成后，
   再次命令行运行 npm run register 这一步是生成token
   检查tokens.txt的行数 是否和emails.txt的行数一致
   ```
6.根据token数量 生成对应的硬件设备号
   ```bash
   npm run setup
   ```
7.修改 proxy.txt 代理的数量和 tokens的数量/email数量保持一致
8. 运行:
   ```bash
   npm run start，如果后台运行请执行 nohup npm run start &
   ```
9.查看运行日志
   ```
   tail -f -n 1000 nohup.out
   ```
