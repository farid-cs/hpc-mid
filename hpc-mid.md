# XWiki installation
## System update (optional)
1. Open your favourite terminal emulator.
2. Run following commands:

```sh
    sudo apt update && sudo apt upgrade
```
3. When asked to confirm press Enter.
4. Wait for update to finish. You should see output like this:
    ![System update](system-update.png)
## Jetty installation
1. Install Java Runtime Environment

```sh
    sudo apt install default-jre
```
    ![JRE installation](install-jre.png)
2. Download jetty from [jetty.org](https://jetty.org/download.html)
    ![jetty website](jetty-website.png)
3. I will download it into current directory using wget
```sh
    wget https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.24/jetty-home-10.0.24.tar.gz
```
    ![wget jetty](download-jetty.png)
5. Create Java and Java/jetty-base folders
```
    mkdir -p Java/jetty-base
```
4. Extract the downloaded file into Java folder
```
    cd Java
    tar -xvf jetty-home-10.0.24.tar.gz
```
