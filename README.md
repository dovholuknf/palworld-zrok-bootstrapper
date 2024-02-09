This repository is meant to help people use `zrok` to run [Palworld](https://store.steampowered.com/app/1623730/Palworld/).

### Prerequisites
* follow the [Palworld tech guide](https://tech.palworldgame.com/dedicated-server-guide) to install the Palworld dedicated server
* download [the latest zrok for windows](https://github.com/openziti/zrok/releases/latest) (zrok_0.4.23_windows_amd64.tar.gz as of feb 9 2024)
* use windows explorer (win11+) or 7zip or something to ungzip and untar the download
* put the zrok.exe somewhere you can find, for example `c:\zrok\zrok.exe`
* invite yourself to zrok using: `zrok invite` (see the [official doc for help](https://docs.zrok.io/docs/getting-started/#generating-an-invitation))

### On the Palworld server:
* `zrok enable` the server. see [Enabling Your zrok Environment](https://docs.zrok.io/docs/getting-started/#enabling-your-zrok-environment)
* download: [the start-server script](https://raw.githubusercontent.com/dovholuknf/palworld-zrok-bootstrapper/main/start-server.ps1)
* edit the script and update the PATH_TO_ZROK with the location of your zrok.exe
* run `start-server.ps1` (the script is not signed, research this if you don't understand it):

      powershell.exe -ExecutionPolicy Bypass -File start-server.ps1

### On the Palworld clients:
* `zrok enable` the client. see [Enabling Your zrok Environment](https://docs.zrok.io/docs/getting-started/#enabling-your-zrok-environment)
* download [the start-client script](https://raw.githubusercontent.com/dovholuknf/palworld-zrok-bootstrapper/main/start-client.ps1)
* update the start-client sciprt with the path to zrok
* run `start-client.ps1` (the script is not signed, research this if you don't understand it):

	  powershell.exe -ExecutionPolicy Bypass -File start-client.ps1
	  