## WSL
A. Enable in Windows features:
	 [ x ] Windows Subsystem for Linux
B. Update WSL:
	 `wsl --update`
C. Install Ubuntu:
	 `wsl --install -d Ubuntu`
D. Export Ubuntu image:
	 `wsl --export Ubuntu D:\ubuntu.tar`
E. Unregister current Ubuntu:
	 `wsl --unregister Ubuntu`
F. Import temporary Ubuntu tar:
	 `wsl --import Ubuntu D:\Ubuntu D:\ubuntu.tar`
G. Configure default user:
	 `ubuntu config --default-user __an_username`
## Docker
A. Download Docker Desktop installer for Windows (https://www.docker.com/products/docker-desktop/)
B. Open Terminal:
	`PS C:\Users\__an_user\Downloads\Docker Desktop Installer.exe >`
C. Install Docker using start command and installer:
	`start /w "" "Docker Desktop Installer.exe" install -accept-license  --installation-dir=D:\Docker\Docker --wsl-default-data-root=D:\Docker\wsl-data --windows-containers-default-data-root=D:\Docker\win-data`

## Checking points
A. `> docker -v` in Windows PowerShell equals `$docker -v` in Ubuntu distro WSL
B. `$ which docker` (-> /usr/bin/docker) and `ls /usr/bin/docker`is a link to /mnt/wsl/docker-desktop/cli-tools/usr/bin/docker

## Misc
A. Vscode has good integrations for wsl and docker.
B. Avoid coding on windows file with ubuntu (locate the Projects dir in home directory)





