To install Ngrok on Ubuntu 20.04 or later, you can follow these steps:

ngrok is a cross-platform application that enables developers to expose a local development server to the Internet with minimal effort.

1. Open your terminal:

   You can press `Ctrl+Alt+T` as a shortcut or search for "Terminal" in the applications menu.

2. Download Ngrok:

   You can download the Ngrok binary from the official website. To do this, you can use the `wget` command:

   ```bash
   wget https://bin.equinox.io/c/4VmDzA7iaHb/ngrok-stable-linux-amd64.zip
   ```

   This command will download the Ngrok binary for Linux.

3. Unzip the Ngrok binary:

   Next, unzip the downloaded file:

   ```bash
   unzip ngrok-stable-linux-amd64.zip
   ```

4. Move the Ngrok binary to a directory in your PATH:

   You can place the Ngrok binary in a directory that is in your system's PATH, making it easily accessible. The `/usr/local/bin` directory is a good choice:

   ```bash
   sudo mv ngrok /usr/local/bin/
   ```

5. Make the Ngrok binary executable:

   Ensure that the Ngrok binary has the execute permission:

   ```bash
   sudo chmod +x /usr/local/bin/ngrok
   ```

6. Authenticate with Ngrok:

   To use Ngrok, you need to create an account and get an authentication token from the Ngrok website (https://dashboard.ngrok.com/get-started). Once you have the token, you can authenticate with Ngrok by running the following command in your terminal:

   ```bash
   ngrok authtoken YOUR_AUTH_TOKEN
   ```

   Replace `YOUR_AUTH_TOKEN` with the token you obtained from the Ngrok website.

Now, Ngrok is installed and configured on your Ubuntu system. You can start using it to expose local services to the internet by running commands like `ngrok http 80` or `ngrok tcp 22`, depending on your specific use case.

$ ngrok authtoken xx
Authtoken saved to configuration file: .ngrok2/ngrok.yml
$ ngrok tcp 3306

