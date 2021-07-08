# Introdução ao Sistema Operacional

**Diretórios**

 Diretório | Descrição|
-----------|----------|
 \               | Diretório Raiz. |
 \bin\           | Contém repositórios binários... executáveis e tem os principais programas. |
 \boot\          | Contém informações sobre o boot. |
 \der\           | Informações de Placa(Vídeo, Áudio).|
 \etc\           | Configuração. |
 \home\          | Usuários, cada novo usuário criasse uma pasta para ele nesse diretório. |
 \lib\           | Contém as bibliotecas. |
 |media ou \mnt\ | Montagem e dispositivos. |
 \opt\           | Programas não oficiais. |
 \sbin\          | cmd admin. |
 \srv\           | Serviços. |
 \usr\           | Usuários. |
 \var\           | Históricos, Email. |
 \root\          | Arquivos importantes do root. |
 \proc\          | Virtual pelo kernel. |

## Parte Prática - 1

"Use | more no final do comando, caso ele tenha uma saída grande para repaginar a saída."

Comandos importantes:

- lspci: Mostra todos os hardware conectados via pci.
- lsusb: Mostra todos os dispositivos usb.
- arch: Mostra a arquitetura.
- uname: Mostra o nome do kernel.
- uname -r: Versão do kernel.
- free: Memória fisica e swap.
- du -h ~: todos os diretórios e quanto pesa.

 ## Parte Prática - 2

 "Use o --help para verificar as informações dos comandos."

 cat \etc\psswd | more - mostra todos os usuários do sistema.
 reboot - reinicia o sistam.
