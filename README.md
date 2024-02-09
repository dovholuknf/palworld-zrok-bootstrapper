This repository is meant to help people use `zrok` to run [Palworld](https://store.steampowered.com/app/1623730/Palworld/).

### Prerequisites
* follow the [Palworld tech guide](https://tech.palworldgame.com/dedicated-server-guide) to install the Palworld dedicated server
* download [the latest zrok for windows](https://github.com/openziti/zrok/releases/latest) (zrok_0.4.23_windows_amd64.tar.gz as of feb 9 2024)
* use windows explorer (win11+) or 7zip or something to ungzip and untar the download
* put the zrok.exe somewhere you can find, for example `c:\zrok\zrok.exe`
* invite yourself to zrok using: `zrok invite`. see https://docs.zrok.io/docs/getting-started/#generating-an-invitation

### On the Palworld server:
* `zrok enable` the server. see [Enabling Your zrok Environment](https://docs.zrok.io/docs/getting-started/#enabling-your-zrok-environment)
* download: [the start-server script](https://raw.githubusercontent.com/dovholuknf/palworld-zrok-bootstrapper/main/start-server.ps1)
* edit the start-server script and update the PATH_TO_ZROK with the location of your zrok.exe
* run `start-server.ps1` (the script is not signed, research this if you don't understand it):

      powershell.exe -ExecutionPolicy Bypass -File start-server.ps1

* after `zrok` starts, there will be a private token that you need to distribute to the people you want to allow to access the Palworld server:
* ![image](https://github.com/dovholuknf/palworld-zrok-bootstrapper/assets/46322585/2774937f-e474-4d08-89ec-d50fd5b70d50)

### On the Palworld clients:
* `zrok enable` the client. see [Enabling Your zrok Environment](https://docs.zrok.io/docs/getting-started/#enabling-your-zrok-environment)
* download [the start-client script](https://raw.githubusercontent.com/dovholuknf/palworld-zrok-bootstrapper/main/start-client.ps1)
* update the start-client script and update the PATH_TO_ZROK with the location of your zrok.exe
* run `start-client.ps1` (the script is not signed, research this if you don't understand it):

	  powershell.exe -ExecutionPolicy Bypass -File start-client.ps1
* when the `start-client.ps1` script executes, you'll be prompted to enter the secret token from the server:
  ![image](https://github.com/dovholuknf/palworld-zrok-bootstrapper/assets/46322585/0f8ab83d-f81e-40d3-87f8-fed81d47f25c)

### YouTube Video Overview:
[<img src="https://img.youtube.com/vi/Sq43hp6n9rE/hqdefault.jpg">](https://youtu.be/Sq43hp6n9rE)
	  
