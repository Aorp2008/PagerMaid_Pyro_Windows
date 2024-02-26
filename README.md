# 最新一次更新时间: 2024/2/26

## 预备软件:
- python3
- git 

## 开始搭建

1. 克隆 PagerMaid-Pyro 仓库到本地：
   ```
   git clone https://gitlab.com/Xtao-Labs/PagerMaid-Pyro 
   ```

2. 进入 PagerMaid-Pyro 目录：
   ```
   cd PagerMaid-Pyro
   ```

3. 创建并激活 Python 虚拟环境：
   ```
   python -m venv venv
   venv\Scripts\activate
   ```

4. 升级 pip 并安装依赖：
   ```
   python -m pip install --upgrade pip
   pip install -r requirements.txt
   ```

5. 复制配置文件并编辑：
   ```
   copy config.gen.yml config.yml
   notepad config.yml
   ```

6. 可选：配置 API：
   ```
   log: "False"
   log_chatid: "503691334"
   proxy_addr: ""
   proxy_port: ""
   http_addr: ""
   http_port: ""
   mtp_addr: ""
   mtp_port: ""
   mtp_secret: ""
   ```

7. 启动 Pagermaid：
   ```
   python -m pagermaid
   ```
8. 输入手机号码，按照提示确认手机号码是否正确，并输入 Telegram APP 收到的验证码。
```Enter phone number or bot token:    #此处填入手机号
Is "+18888888888" correct? (y/N):    # 号码显示正确输入 y ,错误输入 n
The confirmation code has been sent via Telegram app
Enter confirmation code:    # 此处输入 Telegram APP 中收到的验证码
# 如果设置了两步验证，则会出现以下提示
The two-step verification is enabled and a password is required
Password hint: None
Enter password (empty to recover):    # 此处输入两步验证密码
```

出现已启动提示，代表登录成功，此时可以去 Telegram 任意聊天发送 ,help 进行测试。
