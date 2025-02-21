# AutoGen 
[AutoGen 0.4 code repository](https://github.com/microsoft/autogen?tab=readme-ov-file)
AutoGen is a framework for creating multi-agent AI applications that can act autonomously or work alongside humans.

## Update WSL Ubuntu
1. Check the current version:
- Open your WSL terminal.
- Type the command cat /etc/os-release to see the current version of Ubuntu2.

2. Update and upgrade packages:
- Run the following commands to update and upgrade your packages:
```
  sudo apt update
  sudo apt upgrade
```

3. Install the update-manager-core package:
- If it's not already installed, run:
```
  sudo apt install update-manager-core
```

4. Edit the release-upgrades file:
- Open the file /etc/update-manager/release-upgrades in a text editor and ensure the line Prompt=lts is uncommented2.

5. Start the upgrade process:
- Run the command:
```
sudo do-release-upgrade -d
```

6. Verify the new version:
- After the upgrade is complete, you can verify the new version by running:
```
cat /etc/os-release
```

## Update Python

1. Check the current version:
- Open your WSL terminal.
- Type the command python --version or python3 --version to see the current version of Python installed1.

2. Update and upgrade packages:
- Run the following commands to update and upgrade your packages:
```
  sudo apt update
  sudo apt upgrade
```

3. Install Python 3.11:
- Run the command:
```
  sudo apt install python3.11
```

4. Update alternatives:
- To set Python 3.11 as the default version, run:
```
  sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.11 1
  sudo update-alternatives --config python3
```

5. Verify the new version:
- After the upgrade is complete, you can verify the new version by running:
```
  python3 --version
```

## Get Latest Code from Github

## AutoGen install
```
  # Install AgentChat and OpenAI client from Extensions
  pip install -U "autogen-agentchat" "autogen-ext[openai]"
```



