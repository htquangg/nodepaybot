# Nodepay BOT

## For suggestions or to report a bug, please contact [telegram](https://t.me/al3xhuynh)
### But before, check the status of [Nodepay](https://app.nodepay.ai/dashboard)

# Setup
1. [Download Docker Desktop](https://www.docker.com/products/docker-desktop).
2. Login to [Nodepay](https://app.nodepay.ai/dashboard).
3. Open `Developer Tools` and go to `Application(Chrome)` / `Storage(Firefox)`.
4. Go to `Local Storage` > `https://app.nodepay.ai` and copy the value of `np_webapp_token` OR `np_token` (The big array of random numbers and letters). Token lifetime is 7 days.
5. Replace `NP_COOKIE` with the value that you copied.
6. Open CMD and use the Docker Run command of the built image from Docker Hub.
7. Check and Manage the app from Docker Desktop > Containers.
8. If you're stuck at checking login information, repeat steps 2 to 6.

## Installation

1. Clone the repository:

   - Open your terminal or command prompt.
   - Navigate to the directory where you want to install the bot.
   - Run the following command:
     ```
     git clone https://github.com/htquangg/nodepaybot.git
     ```
   - This will create a new directory named `nodepaybot` with the project files.

2. Navigate to the project directory:

   - Change into the newly created directory:
     ```
     cd nodepaybot
     ```

3. Open the `data.txt` file in a text editor and add your account tgWabAppData, one per line:

   ```
   np_token_1
   np_token_2
   np_token_3
   ```

4. If you need to use proxies, fill in the `proxy.txt` file with your proxy addresses, one per line. If not, you can leave this file empty. [example](proxy-example.txt)

5. Run docker
```
docker build -t nodepay:latest . && \
docker run -d \
  --name nodepay-bot\
  --restart unless-stopped \
  nodepay:latest
```

## Disclaimer

This bot is for educational purposes only. Use it at your own risk and make sure you comply with the terms of service of the Nodepay platform.

## License

See the [LICENSE](https://github.com/htquangg/nodepaybot/blob/main/LICENSE) file for more info.

## 🎁 Donate

<div style="display: flex; gap: 20px;">
  <img src="https://raw.githubusercontent.com/htquangg/assets/main/qr_momo.jpg" alt="QR Momo" height="340" />
</div>
