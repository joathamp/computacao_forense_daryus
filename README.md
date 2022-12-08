Laboratório - Analise Forense em Linux - Daryus
=================================================

Repositório para armazenar os arquivos referentes ao Laboratório do curso de Analise Forense em Ambientes Linux e IOS da [Daryus][1]

Dependências
------------

Para a criação do laboratório é necessário ter pré instalado os seguintes softwares:

* [Git][2]
* [VirtualBox][3]
* [Vagrant][5]

> Para máquinas com Windows aconselhamos o uso do proprio Powershell e que as instalações dos softwares são feitas da maneira tradicional

> Para as máquinas com MAC OS aconselhamos, se possível, que as instalações sejam feitas pelo gerenciador de pacotes **brew**.

Laboratório
-----------

O Laboratório será criado utilizando o VirtualBox ou em alguns casos o [Vagrant][7]. Ferramenta para criar e gerenciar ambientes virtualizados (baseado em Inúmeros providers) com foco em automação.

Nesse laboratórios, estara um ou varios arquivos [Vagrantfile][8], sera criada a distribuicao Kali Linux com as configuracoes a seguir:

Nome       | vCPUs | Memoria RAM | IP            | S.O.¹           | Script de Provisionamento²
---------- |:-----:|:-----------:|:-------------:|:---------------:| -----------------------------
Kali       | 1     | 3072MB      | 192.168.56.10 | Kali Linux      | 

> **¹**: Esses Sistemas operacionais estão sendo utilizado no formato de Boxes, é a forma como o vagrant chama as imagens do sistema operacional utilizado.

Criação do Laboratório 
----------------------

Para criar o laboratório é necessário fazer o `git clone` desse repositório e, dentro da pasta baixada realizar a execução do `vagrant up`, conforme abaixo:

```bash
git clone https://github.com/joathamp/computacao_forense_daruys
cd computacao_forense_daryus/
vagrant up
```

_O Laboratório **pode demorar**, dependendo da conexão de internet e poder computacional, para ficar totalmente preparado._


Por fim, para melhor utilização, abaixo há alguns comandos básicos do vagrant para gerencia das máquinas virtuais.

Comandos                | Descrição
:----------------------:| ---------------------------------------
`vagrant init`          | Gera o VagrantFile
`vagrant box add <box>` | Baixar imagem do sistema
`vagrant box status`    | Verificar o status dos boxes criados
`vagrant up`            | Cria/Liga as VMs baseado no VagrantFile
`vagrant provision`     | Provisiona mudanças logicas nas VMs
`vagrant status`        | Verifica se VM estão ativas ou não.
`vagrant ssh <vm>`      | Acessa a VM
`vagrant ssh <vm> -c <comando>` | Executa comando via ssh
`vagrant reload <vm>`   | Reinicia a VM
`vagrant halt`          | Desliga as VMs

> Para maiores informações acesse a [Documentação do Vagrant]

[1]: https://https://www.daryus.com.br/
[2]: https://git-scm.com/downloads
[3]: https://www.virtualbox.org/wiki/Downloads
[5]: https://www.vagrantup.com/downloads
[6]: https://cygwin.com/install.html
[7]: https://www.vagrantup.com/
[8]: ./Vagrantfile

- Msc. Joatham Pedro
- Bacharel em Ciencia da Computacao
- Pós-Graduado em Redes de Computadores
- Mestre em Redes e Computação
- Analista Sênior de Segurança da Informação - 4Linux
- Instrutor MBA Cybersecurity Gov TI - FATEC Cuiabá
- Instrutor  MBA Cybersecurity - IMPACTA
- Instrutor Pos Graduacao Computação Forense - Daryus
- Linux Professional Institute I
- Linux Professional Institute II
- Linux Professional Institute III - Security
- Data Center Technical Specialist
- Novell Certified Linux Administrator (CLA)
- Computer Hacking Forensic Investigator - C|HFI
- Certified Ethical Hacker - C|EH
- Certified Incident Handler - EC|IH
- Exin Ethical Hacker - EXIN
- DevOps Essential Professional - DEPC
- youtube.com/eaiqualteupapo

- https://beacons.ai/qualteupapo
