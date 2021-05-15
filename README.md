# Hospedagem de aplicações web

*******
Sumário
 1. [Infraestrutura](#infraestrutura)
 2. [Serviços de hospedagem](#servicos)
 3. [Configurações e acesso ao servidor](#servidor)
 4. [Aplicação web](#aplicacao)
 5. [Links](#links)

*******

<div id='infraestrutura'/>

## Infraestrutura

Aplicações robustas demandam planejamento, é importante saber sobre questões de segurança, desempenho e o quanto sistema vai precisar de memória. É possível hospedar uma aplicação em um servidor físico que é designado a um único usuário. Também utilizar de máquinas virtuais (vms) para criar o próprio servidor, as vms são ambientes de virtualização que simulam um ou vários sistemas operacionais (so). 

Máquinas virtuais:

- [VirtualBox](https://www.virtualbox.org/)
- [VMware](https://www.vmware.com/br.html)

Ao longo da criação do servidor algumas especificações de hardware, software e rede poderão ser definidas:

    Memória
    Processador
    Conexão de rede
    Disco rígido
    Sistema Operacional (SO)

<div id='servicos'/>

## Serviços de hospedagem

Existem diversas plataformas que prestam serviços de hospedagem. As plataformas abaixo são serviços de hospedagem em nuvem, para utilizá-los é preciso pagar, porém algumas dessas oferecem funcionalidades que são gratuitas:

- [DigitalOcean](https://www.digitalocean.com/)
- [IBM](https://www.ibm.com/br-pt)
- [Microsoft Azure](https://azure.microsoft.com/pt-br/) 
- [Amazon Web Services (AWS)](https://aws.amazon.com/pt/)

Como alternativa, a plataforma abaixo permite criar um serviço de hospedagem gratuito:

- [Vagrant](https://www.vagrantup.com/): é um software para gerencia de ambientes de desenvolvimento virtuais combinado ao VirtualBox.

<div id='servidor'/>

## Configurações e acesso ao servidor

O servidor não tem interface e tudo será feito por linha de comando no terminal. Para um servidor funcionar ele precisa das seguintes configurações básicas:

- Nome de usuário
- Host (domínio ou endereço ip)
- Senha (será gerada uma senha aleatória)

O servidor é acessado por meio de um cliente SSH que vai entrar na máquina virtual remotamente. As opções abaixo podem ser usadas para acessar um servidor:

- Linux e Mac: [OpenSSH](https://www.openssh.com/) (muitas vezes já vem instalado)
- Windows: [Putty](https://www.putty.org/)

Comandos de acesso ao servidor:

`$ ssh ssh://usuario@dominio.com:2222` 

ou 

`$ ssh usuario@<endereco-ip-servidor>`

Outras configurações que podem ser feitas para o servidor:

    Privilégios de acesso do usuários e segurança do servidor
    Ufw ferramenta de Firewall - analisa o trafego da rede e ajuda a gerenciar o que pode ser executado no servidor 
    Banco de dados (MySQL, MariaDB, PostgreSQL, Oracle...)
    
<div id='aplicacao'/>

## Aplicação web

**Tecnologias:** A tecnologia base de um sistema web é o HTML que pode ser combinado junto ao CSS e JavaScript essas tecnologias compõe o frontend (parte de interação com o usuário). A estrutura do sistema é desenvolvido por meio das linguagens de programação, Python, JavaScript, PHP e entre outras que são parte do backend (parte não visivel ao usuário). Todas essas tecnologias podem ser usadas com os frameworks, Flask, Django, Vue, React, Angular e vários outros.

**Código-fonte:** A ferramenta [Git](https://git-scm.com/) ajuda na organização e controle de versão dos códigos. E o [GitHub](https://github.com/) é uma plataforma para hospedagem do código-fonte. O Git junto ao GitHub ajudam no processo de desenvolvimento do sistema, além de simplificar a instalação do projeto em qualquer ambiente.

<div id='links'/>

## Links
