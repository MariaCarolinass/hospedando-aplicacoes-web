# Hospedagem de aplicações web

*******
Sumário
 1. [Infraestrutura](#infraestrutura)
 2. [Serviços de hospedagem](#servicos)
 3. [Configuração e acesso ao servidor](#servidor)
 4. [Aplicação web](#aplicacao)
 5. [Links](#links)

*******

<div id='infraestrutura'/>

## Infraestrutura

Aplicações robustas demandam planejamento, é importante saber sobre questões de segurança, desempenho e o quanto o sistema vai precisar de memória. É possível hospedar uma aplicação em um servidor físico que é designado a um único usuário. Também utilizar de máquinas virtuais (vms) para criar o próprio servidor, as vms são ambientes de virtualização que simulam um ou vários sistemas operacionais (so). 

Máquinas virtuais:

- [VirtualBox](https://www.virtualbox.org/)
- [VMware](https://www.vmware.com/br.html)

Ao longo da criação do servidor algumas especificações de hardware, software e rede devem ser definidas:

    Memória
    Processador
    Conexão de rede
    Disco rígido
    Sistema Operacional (SO)

<div id='servicos'/>

## Serviços de hospedagem

Existem diversas plataformas que oferecem serviços de hospedagem, muitas delas usam o conceito de computação em nuvem, são elas:

- [DigitalOcean](https://www.digitalocean.com/)
- [IBM](https://www.ibm.com/br-pt)
- [Microsoft Azure](https://azure.microsoft.com/pt-br/) 
- [Amazon Web Services (AWS)](https://aws.amazon.com/pt/)

Como alternativa as plataformas pagas:

- [Vagrant](https://www.vagrantup.com/): serviço de hospedagem combinado ao VirtualBox

### Servidores web (HTTP):

Os servidores abaixo são responsáveis por responderem às solicitações (HTTP) dos clientes no navegador:

 - [Apache](https://www.apache.org/)
 - [Gunicorn](https://gunicorn.org/)
 - [Nginx](https://nginx.org/) (servidor intermediário): responde às requisições de clientes que solicitam recursos de outros servidores (E-mail: IMAP, POP3)

<div id='servidor'/>

## Configuração e acesso ao servidor

O servidor não tem interface e tudo será feito através de linha de comando no terminal. As seguintes configurações básicas abaixo são necessárias para o servidor funcionar:

    Nome do usuário
    Host (domínio ou endereço IP)
    Senha (será gerado uma chave aleatória)

Uma das formas de acessar o servidor é utilizando um cliente SSH, que vai entrar no servidor remotamente. 

Cliente SSH:

- Linux e Mac: [OpenSSH](https://www.openssh.com/)
- Windows: [Putty](https://www.putty.org/)

Comandos para acessar o servidor:

`$ ssh ssh://usuario@dominio.com:porta` 

ou 

`$ ssh usuario@<endereco-ip-servidor>`

Outras configurações do servidor:

- Permissões e privilégios de usuários
- Segurança
- Firewall (ufw) - analisa o trafego da rede e gerência o que pode ser executado no servidor 
- Banco de dados (MySQL, MariaDB, PostgreSQL, Oracle...)
    
<div id='aplicacao'/>

## Aplicação web

**Tecnologias:** A tecnologia base de um sistema web é o HTML que pode ser combinado junto ao CSS e JavaScript essas tecnologias compõe o frontend (parte de interação com o usuário). A estrutura do sistema é desenvolvido por meio das linguagens de programação, Python, JavaScript, PHP e entre outras que são parte do backend (parte não visivel ao usuário). Todas essas tecnologias podem ser usadas com os frameworks, Flask, Django, Vue, React, Angular e vários outros.

**Código-fonte:** A ferramenta [Git](https://git-scm.com/) ajuda na organização e controle de versão dos códigos. E o [GitHub](https://github.com/) é uma plataforma para hospedagem do código-fonte. O Git junto ao GitHub ajudam no processo de desenvolvimento do sistema, além de simplificar a instalação do projeto em qualquer ambiente.

<div id='links'/>

## Links
