# Apostila Linux LPI Essentials

### By: Matheus Barbosa Ribeiro

---

# Kernel

---

Em computação, **Kernel** é o componente central do sistema operacional. Ele serve de ponte entre o hardware, aplicativos e processamentos
![KernelLayoutsvg](https://upload.wikimedia.org/wikipedia/commons/8/8f/Kernel_Layout.svg)

As responsabilidades do Kernel incluem gerenciar os recursos do sistema (a comunicação entre componentes de hardware e software). Essas tarefas e gerenciamentos são feitos de formas diferentes dependendo do Kernel do seu sistema operacional.

# Kernel Monolítico

---

Em um kernel monolítico, todos os serviços do sistema operacional rodam junto com a linha de execução principal do próprio, portanto, se encontram na mesma área de memória. Essa abordagem permite um acesso vasto e poderoso ao hardware.

> O desenvolvedor do UNIX (Ken Thompson), defende que "é mais fácil de implementar um kernel monolítico"

As principais desvantagens do kernel monolítico são as dependências entre os componenetes do sistema e o fato de que quando temos um kernel grande a manutenção é penosa.

# Microkernels

---

 Essa abordagem consistem em definir abstrações simples sobre o hardware, com um conjunto de chamadas de sistema para implementar serviços mínimos como:

- Gerenciamento de memória;
- Multitarefas;
- Comunicação entre processos.

Outros serviços, incluindo aqueles normalmente fornecidos por um kernel monolítico, são implementados em programas de espaço de usuário, conhecidos como servidores.
Microkernels são mais fáceis de manter do que os monolíticos, mas, um grande número de chamadas de sistema podem desacelerá-lo visto eles geralmente geram mais degradação na performance do que uma simples chamadas de função.

Um microkernel permite a implementação e uso de diferentes sistemas operacionais, além de tornar possível alterar dinamicamente entre SO's e/ou manter mais de um deles ativos simultâneamente.

## Entendendo

Nesta apostila vamos falar principalmente do Linux, mas, para isso foi preciso uma breve explicação do que é um Kernel.
Agora vamos começar a entender essa belezinha!

# Linux

---

O Linux é um kernel monolítico de código aberto(open source de licensa GPL) para sistemas operacionais do tipo UNIX, e foi desenvolvido para ambos os sistemas computacionais, seja computadores pessoais ou servidores, normalmente na forma de distribuições Linux.
Ele pode ser encontrado em diversos dispositivos como: 

- Rroteadores;
- Receptores de televisão;
- Smart TVs;
- Android;
- Etc.

Estes dispositivos utilizam serviços providos pelo kernel do Linux para implementar as suas funcionalidades.

O kernel do Linux foi, originalmente, escrito por **Linus Torvalds** do Departamento de Ciência da Computação da Universidade de Helsinki, Finlândia, com a ajuda de vários programadores voluntários através da Usenet (uma espécie de sistema de listas de discussão).

Linus Torvalds começou o desenvolvimento do kernel como um projeto particular, inspirado pelo seu interesse no Minix, um pequeno sistema UNIX desenvolvido por Andrew S. Tanenbaum. Ele limitou-se a criar, nas suas próprias palavras, "um Minix melhor que o Minix" ("a better Minix than Minix").

## GPL

GNU General Public License (Licença Pública Geral GNU), GNU GPL ou simplesmente GPL, é a designação da licença de software idealizada por Richard Matthew Stallman em 1989, no âmbito do projeto GNU. Richard Stallman originalmente criou a licença para o Projeto GNU de acordo com as definições de software livre da Free Software Foundation.

Sendo uma licença copyleft, trabalhos derivados de um produto originalmente licenciado pela GPL só podem ser distribuídos se utilizarem a mesma licença. Isso é diferente das licenças mais permissivas como a licença BSD e a licença MIT, que possuem exigências mais simples.
Historicamente, as licenças GPL são utilizadas por projetos de software livre e de código aberto.

> **Projeto GNU:** 
> GNU é um sistema operacional tipo Unix cujo objetivo desde sua concepção é oferecer um sistema operacional completo e totalmente composto por software livre
> **Free Software Foundation:**
> A Free Software Foundation (FSF, Fundação para o Software Livre) é uma organização sem fins
> lucrativos, fundada em 4 de Outubro de 1985 por Richard Stallman e que se dedica a eliminação de restrições sobre a cópia, estudo e modificação de programas de computadores – bandeiras do movimento do software livre, em essência. Faz isso promovendo o desenvolvimento e o uso de software livre em todas as áreas da computação mas, particularmente, ajudando a desenvolver o sistema operacional GNU e suas ferramentas.

### Em termos gerais, a GPL baseia-se em 4 liberdades:

1. A liberdade de executar o programa, para qualquer propósito (liberdade nº 0)
2. A liberdade de estudar como o programa funciona e adaptá-lo às suas necessidades (liberdade nº 1). O acesso ao código-fonte é um pré-requisito para esta liberdade.
3. A liberdade de redistribuir cópias de modo que você possa ajudar ao seu próximo (liberdade nº 2).
4. A liberdade de aperfeiçoar o programa e liberar os seus aperfeiçoamentos, de modo que toda a comunidade beneficie deles (liberdade nº 3). O acesso ao código-fonte é um pré-requisito para esta liberdade.

# Algumas Distribuições com kernel linux

---

## Debian:

![Debian-logo](https://upload.wikimedia.org/wikipedia/commons/4/4a/Debian-OpenLogo.svg)
O Debian é um sistema operacional composto inteiramente de software livre e mantido oficialmente pelo Projeto Debian(comunidade). O projeto recebe, ainda, apoio de outros indivíduos e organizações de todo o mundo. O grupo distribui kernels Unix-like, como o Debian GNU/kFreeBSD e o Debian GNU/Hurd. O Debian é especialmente conhecido pelo seu sistema de gestão de pacotes, chamado APT, que permite atualizações relativamente fáceis a partir de versões anteriores, a instalação quase sem esforço de novos pacotes e a remoção limpa de pacotes antigos.

## Ubuntu

![Ubuntu-logo](https://upload.wikimedia.org/wikipedia/commons/7/76/Ubuntu-logo-2022.svg)
Ubuntu é um sistema operacional de código aberto, construído a partir do kernel Linux, baseado no Debian e utiliza GNOME como ambiente de desktop de sua mais recente versão com suporte de longo prazo (LTS). Esta distribuição Linux é desenvolvida pela Canonical Ltd.
Geralmente é executado em computadores pessoais e também é popular em servidores de rede, geralmente executando a versão Ubuntu Server, com recursos de classe empresarial.

## Red Hat

![Red Hat - logo](https://upload.wikimedia.org/wikipedia/pt/e/ec/Red_Hat.jpg)
A Red Hat, Inc. é uma empresa dos Estados Unidos, que disponibiliza soluções baseadas no sistema operacional GNU/Linux, incluindo o Red Hat Enterprise Linux, além de soluções de software.

## Fedora

![Fedora-logo](https://upload.wikimedia.org/wikipedia/commons/8/8f/Fedora_logo_%282021%29.svg)
O Fedora Linux existe desde 2003, e seu desenvolvimento e suporte é oferecido pela comunidade do Projeto Fedora. Após ter descontinuado o sistema operacional Red Hat Linux, a Red Hat patrocina o desenvolvimento do sistema operacional Fedora, se envolvendo no desenvolvimento de vários programas disponíveis para o mesmo, que são eventualmente adicionados para o repositório do Red Hat Enterprise Linux, que é a distribuição Linux atual da empresa.

## CentOS

![centOS - logo](https://upload.wikimedia.org/wikipedia/commons/b/bf/Centos-logo-light.svg)
O CentOS, abreviação de Community ENTerprise Operating System, é uma distribuição Linux de classe corporativa derivada de códigos fonte gratuitamente distribuídos pela Red Hat Enterprise Linux e mantida pelo CentOS Project.

## Scientific Linux

![scientific-logo](https://upload.wikimedia.org/wikipedia/commons/b/b1/Scientific_Linux_logo_and_wordmark.svg)
Scientific Linux é uma distribuição Linux padronizado pelo Fermi National Accelerator Laboratory ou Fermilab (Illinois/USA). Ele é um sistema operacional livre e de código aberto baseado no Red Hat Enterprise Linux (RHEL).O objetivo principal para o desenvolvimento do Scientific Linux foi disponibilizar uma distribuição de Linux para alguns laboratórios e universidades, que corresponde com as necessidades para experimentos físicos de alta energia e intensidade.

## Linux Mint

![mint-logo](https://upload.wikimedia.org/wikipedia/commons/6/6b/Linux_Mint_Logo_%28until_2021%29.svg)
Linux Mint é uma distribuição Linux irlandesa. Possui duas versões: uma baseada em Ubuntu (com o qual é totalmente compatível e partilha os mesmos repositórios) e outra versão baseada em Debian. Suporta muitos idiomas, incluindo a língua portuguesa, e utiliza o Cinnamon como seu principal ambiente de desktop.

Esforça-se para ser um "sistema operacional moderno, elegante e confortável, que é poderoso e fácil de usar" e possui suporte de mídia pronto para o uso, incluindo alguns softwares proprietários e vem com uma variedade de aplicativos gratuitos e de código aberto.

## OpenSUSE

![opensuse-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d0/OpenSUSE_Logo.svg/1280px-OpenSUSE_Logo.svg.png)
openSUSE é um sistema operacional baseado no kernel Linux, desenvolvido pela comunidade openSUSE de forma gratuita.
Após adquirir o SUSE Linux em janeiro de 2004, a Novell, uma empresa norte-americana que na década de 1980 ficou famosa por seu sistema operacional de rede (Netware), após o sucesso lançou o SUSE Linux Professional como um projeto 100% código livre, envolvendo a comunidade no processo de desenvolvimento.
O openSUSE é dirigido pela comunidade OpenSUSE Project e patrocinada pela Novell, para desenvolver e manter os componentes das distribuições SUSE Linux 

# Padrões presentes em distribuições que usam o kernel Linux

---

## Filesystem Hierarchy Standard

O Filesystem Hierarchy Standard (padrão para sistema de arquivos hierárquico), ou FHS, define os principais diretórios, e o seu conteúdo, em um sistema operacional Linux ou do tipo Unix.

| Diretório        | Descrição                                                                                                                                                           |
|:----------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| /                | Diretório raiz de toda a hierarquia do sistema de arquivos.                                                                                                         |
| /bin/            | Comandos binários essenciais para todos os usuários (ex: cat, ls, cp)                                                                                               |
| /boot/           | Arquivos do Boot loader (ex: núcleo, initrd).                                                                                                                       |
| /dev/            | Dispositivos (ex: /dev/null).                                                                                                                                       |
| /etc/            | Arquivos de configuração específicos do computador.                                                                                                                 |
| /etc/opt/        | Arquivos de configuração para o /opt/.                                                                                                                              |
| /etc/X11/        | Arquivos de configuração para o X Window System, versão 11.                                                                                                         |
| /etc/sgml/       | Arquivos de configuração para SGML.                                                                                                                                 |
| /etc/xml/        | Arquivos de configuração para XML.                                                                                                                                  |
| /home/           | Diretórios de usuários.(Opcional)                                                                                                                                   |
| /lib/            | Diretório com as bibliotecas essenciais para os arquivos binários contidos nos diretórios /bin/ e /sbin/.                                                           |
| /mnt/            | Sistemas de arquivos "montados" temporariamente.                                                                                                                    |
| /media/          | Pontos de "montagem" para mídia removível, como CD-ROMs (surgiram na versão 2.3 do FHS).                                                                            |
| /opt/            | Pacotes estáticos de aplicações.                                                                                                                                    |
| /proc/           | Sistemas de arquivo virtual, que possui o estado do núcleo e processos do sistema; a maioria dos arquivos é baseada no formato texto (ex: tempo de execução, rede). |
| /root/           | Diretório home para o superusuário (root).(Opcional)                                                                                                                |
| /sbin/           | Arquivos binários para propósito de administração do sistema.                                                                                                       |
| /tmp/            | Arquivos temporários. (Ver também /var/tmp).                                                                                                                        |
| /srv/            | Dados específicos que são servidos pelo sistema.                                                                                                                    |
| /usr/            | Hierarquia secundária para dados compartilhados de usuários, cujo acesso é restrito apenas para leitura.                                                            |
| /usr/bin/        | O mesmo que a hierarquia do topo (/bin), mas contém apenas arquivos não essenciais (que não são necessários para que o sistema funcione ou para a sua recuperação). |
| /usr/include/    | Diretório padrão para arquivos do tipo header.                                                                                                                      |
| /usr/lib/        | O mesmo que a hierarquia do topo (/lib).                                                                                                                            |
| /usr/sbin/       | O mesmo que a hierarquia do topo, mas contém apenas arquivos não essenciais (ex: daemons e serviços de rede).                                                       |
| /usr/share/      | Dados compartilhados que são independentes da arquitetura do computador.                                                                                            |
| /usr/src/        | Código fonte (ex: código fonte do núcleo do sistema).                                                                                                               |
| /usr/X11R6/      | X Window System, Versão 11 R6.                                                                                                                                      |
| /usr/local/      | Hierarquia terciária com dados locais, específicos deste host.                                                                                                      |
| /var/            | Arquivos "variáveis", como logs, base de dados, páginas Web e arquivos de e-mail.                                                                                   |
| /var/lock/       | Arquivos de lock. Utilizados para manter o controle sobre recursos em uso.                                                                                          |
| /var/log/        | Arquivos para log. Utilizado para log de dados em geral.                                                                                                            |
| /var/mail/       | Caixas de email dos usuários do sistema.                                                                                                                            |
| /var/run/        | Contém informação sobre a execução do sistema desde a sua última inicialização. (ex: usuários e daemons em execução).                                               |
| /var/spool/      | Spool para tarefas em espera para execução. (ex: filas de impressão e emails ainda não lidos).                                                                      |
| /var/spool/mail/ | Local para caixas de correio dos usuários. Não deve ser mais utilizada, existe apenas para compatibilidade retroativa.                                              |
| /var/tmp/        | Arquivos temporários. Quando em modo multi-usuário, preferível em relação ao /tmp.                                                                                  |

## Linux Standard Base

Linux Standard Base (LSB), traduzido para Base Padrão do Linux, é um projeto conjunto de diversas distribuições Linux sob a estrutura organizacional da Fundação Linux para padronizar a estrutura de sistemas de software, incluindo a hierarquia de sistema de arquivos usada no sistema operacional. A LSB é baseada na especificação POSIX, na Single UNIX Specification e em diversos outros padrões abertos.

De acordo com a LSB:

> O objetivo da LSB é desenvolver e promover um conjunto de padrões abertos que aumentarão a compatibilidade entre distribuições Linux e permitir que aplicações de software rodem em qualquer sistema compatível, mesmo em formato binário. Ademais, a LSB ajudará a coordenar esforços para recrutar fornecedores de software a portarem e escreverem seus produtos para Sistemas Operacionais Linux.

## Para lembrar:

- Debian: mantida pela comunidade
- Ubuntu: baseado no debian, mantido por uma organização e responsável por popularizar o Linux nos desktops no mundo inteiro
- RedHat Enterprise Linux (RHEL): mantida pela RedHat
- CentOS: baseada no RHEL, sem os programas proprietários da RedHat
- ScientificLinux: distribuição que já vem com softwares específicos para a comunidade de pesquisa
- Mint Linux: uma versão desktop de linux
- Android: existe uma discussão se é realmente um linux ao pé da letra, mas para todos os efeitos ele na prova será considerado uma distribuição linux

# Principais aplicações Open Source do mundo linux

- Firefox
  
  - Mozilla Firefox é um navegador livre e multiplataforma desenvolvido pela Mozilla Foundation com ajuda de centenas de colaboradores. A intenção da fundação é desenvolver um navegador leve, seguro, intuitivo e altamente extensível. Baseado no componente de navegação da Mozilla Application Suite, o Firefox tornou-se o objetivo principal da Mozilla Foundation.
    Cerca de 40% do código do programa foi totalmente escrito por voluntários.

- Thunderbird
  
  - Mozilla Thunderbird é uma aplicação livre e de código aberto, que funciona como cliente de e-mails e notícias, tendo sido produzida pela Mozilla Foundation, a mesma criadora do navegador Mozilla Firefox. Acessa também arquivos XML, Feeds (Atom e RSS), bloqueia imagens, tem filtro anti-spam embutido e um mecanismo que previne golpes por meio das mensagens.

- OpenOffice
  
  - OpenOffice.org é um conjunto de aplicativos OpenSource para escritório, distribuída para os sistemas operacionais Microsoft Windows, Unix, Solaris, Linux e Mac OS X, e mantida pela Apache Software Foundation. O conjunto usa o formato ODF (OpenDocument) — formato homologado como ISO/IEC 26300 e NBR ISO/IEC 26300 — e é também compatível com os formatos do Microsoft Office, além de outros formatos legados.

- LibreOffice
  
  - LibreOffice é uma suíte de aplicativos livres e de código aberto para escritório disponível para Windows, Unix, Solaris, Linux e macOS. A suíte utiliza o formato OpenDocument (ODF - OpenDocument Format) — formato homologado como ISO/IEC 26300 e NBR ISO/IEC 26300 — e é também compatível com os formatos do Microsoft Office, além de outros formatos legados.
  - O LibreOffice surgiu como uma ramificação do projeto original OpenOffice.org, isso ocorreu, por que quando a Oracle comprou a Sun Microsystems (e junto com ela os direitos do OpenOffice.org), alguns desenvolvedores e colaboradores do OpenOffice.org deixaram o projeto controlado pela Oracle para montar o LibreOffice, criando um fork (ramificação) do projeto original.

- GIMP
  
  - GIMP (GNU Image Manipulation Program) é um programa de código aberto voltado principalmente para criação e edição de imagens, e em menor escala também para desenho vetorial.
  - O projeto foi criado em 1995 por Spencer Kimball e Peter Mattis, que o desenvolveram como um projeto para a faculdade. Atualmente, ele é mantido por um grupo de voluntários e licenciado sob a GNU General Public License.

# Aplicações de servidor

- Apache HTTPD
  
  - Apache, é o servidor web OpenSource criado em 1995 por Rob McCool. É a principal tecnologia da Apache Software Foundation, responsável por mais de uma dezena de projetos envolvendo tecnologias de transmissão via web, processamento de dados e execução de aplicativos distribuídos.

- NGINX
  
  - Nginx é um servidor leve de HTTP, proxy reverso, proxy de e-mail IMAP/POP3, feito por Igor Sysoev em 2005, sob licença BSD-like 2-clause. O Nginx consome menos memória que o Apache, pois lida com requisições Web do tipo “event-based web server”; e o Apache é baseado no “process-based server”, podendo trabalhar juntos. É possível diminuir o consumo de memória do Apache, passando as requisições Web primeiro no Nginx, assim, o Apache não precisa servir arquivos estáticos, e pode depender do bom controle de cache feito pelo Nginx.

- MySQL
  
  - O MySQL é um sistema de gerenciamento de banco de dados (SGBD), que utiliza a linguagem SQL como interface. É atualmente um dos sistemas de gerenciamento de bancos de dados mais populares da Oracle Corporation, com mais de 10 milhões de instalações pelo mundo.
  
  - Entre os usuários do banco de dados MySQL estão: NASA, Friendster, Banco Bradesco, Dataprev, HP, Nokia, Sony, Lufthansa, U.S. Army, U.S. Federal Reserve Bank, Associated Press, Alcatel, Slashdot, Cisco Systems, Google, entre outros.

- LAMP
  
  - LAMP (Linux, Apache, MySQL, PHP/Perl/Python) é um acrônimo que denota um dos conjuntos de soluções mais comuns para muitas das aplicações mais populares na web. No entanto, LAMP agora se refere a um modelo de conjunto de software genérico e seus componentes são amplamente intercambiáveis.
  
  - Cada letra da sigla representa um de seus quatro blocos de construção de código aberto:
    
    - Linux para o sistema operacional
    
    - Servidor HTTP Apache
    
    - MySQL para o sistema de gerenciamento de banco de dados relacional
    
    - Linguagem de programação PHP, Perl ou Python
      
      > Os componentes dos conjuntos LAMP estão presentes nos repositórios de software da maioria das distribuições Linux.

- NFS
  
  - NFS (acrônimo para Network File System) é um sistema de arquivos distribuídos desenvolvido inicialmente pela Sun Microsystems, Inc., a fim de compartilhar arquivos e diretórios entre computadores conectados em rede, formando assim um diretório virtual.

- SAMBA
  
  - Samba é um programa de computador, utilizado em sistemas operacionais do tipo Unix, que simula um servidor Windows, permitindo que seja feito gerenciamento e compartilhamento de arquivos em uma rede Microsoft.

- POSTFIX
  
  - Postfix é um agente de transferência de e-mails (MTA) livre e de código aberto que encaminha e entrega e-mails, e tem como objetivo ser uma alternativa segura ao Sendmail, muito utilizado em servidores UNIX.
  
  - O software também conhecido como VMailer e IBM Secure Mailer, continua a ser ativamente desenvolvido pelo seu criador e outros contribuidores e é o agente de transferência de e-mails padrão de inúmeros sistemas operativos como o OS X, o Ubuntu, e o NetBSD.

# Usando um sistema linux

---

Vamos usar o Ubuntu como exemplo.

# apt

Vamos aprender como instalar um programa via Terminal de Linux. Como exemplo, iremos instalar um servidor FTP.

O Ubuntu nos disponibiliza um sistema de gerenciamento de pacotes chamado **apt**. Para ver as versões atualizadas dos programas que estão disponíveis para instalação fazemos:

```shell
$ sudo apt-get update
```

> Obs: A opção `upgrade` do `apt-get`, serve para atualizar todo o nosso sistema, atualizando as versões dos pacotes que já estão instalados.
> 
> A opção `show` do comando `apt-cache`, mostra informações sobre um determinado pacote. Aproveite para fazer um teste:
> 
> ```shell
> $ apt-cache show mysql-server-5.6
> ```

Veja que executamos o comando como *root* (`sudo`), isto porque esta é uma tarefa de administração, por isso é necessário que seja feita como *root*, caso não, teremos uma mensagem de permissão negada. Neste passo, o Terminal irá buscar na internet o que existe de novidade nos programas para instalação. Para buscar um programa de servidor FTP podemos fazer:

```shell
$ apt-cache search ftp
```

Este comando busca na lista de pacotes disponíveis, qualquer programa que se encaixe nesse termo de busca, por isso retorna uma longa lista de programas. Sejamos mais restritos na busca e procuremos um servidor específico:

```shell
$ apt-cache search vsftp
```

Achamos um bom servidor FTP, ele nos mostra o nome e uma curta descrição. Para instalar este programa fazemos:

```shell
$ sudo apt-get install vsftpd
```

## Removendo

Para que possamos remover programas, utilizamos o comando `apt-get remove` seguido do nome do programa. Como exemplo, vamos desinstalar o servidor que instalamos.

```shell
$ sudo apt-get remove vsftpd
```

> Para buscar ou instalar os programas o Ubuntu usa listas, essas listas podemos chamá-las de repositórios.
> Podemos vizualizar estes repositórios fazendo: