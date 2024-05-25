#### Vagrant

Projetos e estudos sobre Vagrant.

![Vagrant](https://www.handsonplus.com/wp-content/uploads/2020/12/vagrant-virtualbox-install_00.jpg)

#### Anotações

Vagrant é uma ferramenta para construir e gerenciar ambientes de máquinas virtuais em um único fluxo de trabalho.

- **Gestão de VMs**
- **Automatização**
- **Comando via CLI**

[Vagrant Site](https://developer.hashicorp.com/vagrant)
[Vagrant and Windows Subsystem for Linux - WSL](https://developer.hashicorp.com/vagrant/docs/other/wsl)

#### Arquitetura

- **VagrantFile: Definição da VM**

#### Comandos

- **vagrnat --version**
- **vagrant init**
- **vagrant up**
- **vagrant ssh vm.hostname**

#### Plugins 

- vagrant plugin install vagrant-aws
- vagrant plugin list
- vagrant plugin install vagrant-vbguest --plugin-version 0.21

#### Pontos de Atenção

- Configuarar o .gitignore para ignorar o diretório .vagrant

- O Comando **vagrant destroy** apaga apenas a machina, e não a **box** (arquivo local)

- Toda alteração no script de provisionamento, deve ser seguida de **destroy** e **up**

- Alterações que não alteram o provionamento, pode se executar apenas o **vagrant reload**

- Instalar o módulo **vbguest**