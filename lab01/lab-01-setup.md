# LAB-01

## Pliki do pobrania:

- Virtualbox https://download.virtualbox.org/virtualbox/7.0.10/VirtualBox-7.0.10-158379-Win.exe
- Vargrant https://releases.hashicorp.com/vagrant/2.3.7/vagrant_2.3.7_windows_amd64.msi
- Git https://github.com/git-for-windows/git/releases/download/v2.42.0.windows.2/Git-2.42.0.2-64-bit.exe
- Visual Studio Code https://code.visualstudio.com/download#
- MobaXterm (należy rozpakować przed instalacją) https://download.mobatek.net/2322023060714555/MobaXterm_Installer_v23.2.zip

## Kroki do wykonania:

```
1. uruchomić mobaxterm

2. git clone https://github.com/mkycia/vagrant-k8s-lab

3. cd vagrant-k8s-lab

4. vagrant up --provider virtualbox

5. mkdir ~/.ssh/
   vagrant ssh-config >  ~/.ssh/config

6. ssh k8s-lab

7. minikube status
```