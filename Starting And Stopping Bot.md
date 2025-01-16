# How to Start And Stop The PepeBuldak Bot

1. Navigate to your [AWS EC2 Instance](https://us-east-1.console.aws.amazon.com/ec2/home).
2. Click on the instance ID beside the Instance with the name "pepe-buldak".
3. Click on the "Connect" button at the top right of the page.
4. Click on "Connect" on the page to proceed with the connection.
5. Wait for the console to load.
6. Once the console loads, run the following in order:

```bash
sudo su -
```

```bash
cd pepe
```

7. To start the bot, run:

```bash
pm2 start build/index.js
```

This should start up the bot.

8. To stop the bot, after doing 1 - 6, run:

```bash
pm2 stop all
```
