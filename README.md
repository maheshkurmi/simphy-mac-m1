![Simphy logo](https://user-images.githubusercontent.com/80441425/110777628-56991180-8287-11eb-9f4b-cf282c4d22da.png)
# Simphy java app for Mac M1
After a huge amount of efforts and time, we are proud to announce that SimPHY now works natively on MacOS arm64.
However we could’t still create dmg installer, means Jva will have to be installed.

Native support for the newer Apple chips is still a work in progress, and there is not a native launcher available. However you can manually install a native JRE and use Simphy's jar launcher. Getting this setup working might require some technical skills.

## Follow the steps to get it working
### Installing Azul's JVM
* Head to Azul's site, download the [.dmg package](https://cdn.azul.com/zulu/bin/zulu11.52.13-ca-jre11.0.13-macosx_aarch64.dmg) and install it.
* Ensure that `/usr/libexec/java_home` points to `/Library/Java/JavaVirtualMachines/zulu-11.jdk/Contents/Home` (if not, a restart should do the trick).

### Installing and running Simphy jar App
* download this repository and extract app directory
* double click `simphy.jar` in app folder to run application
* if it does’t work, open terminal, navigate to app directory then run command `java -jar simphy.jar`
* If still it does’t work, try restarting your computer or double check if it is using the correct JVM by using the java --version command on the terminal.
