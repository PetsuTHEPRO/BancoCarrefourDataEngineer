# Aula 7 - Como adicionar Usuário

- adduser (sudo): Cria um usuário.
- su (nome): Muda de usuário.
- passwd (nome): Muda senha.

> ZENIT POLAR: Procedimento de criar códigos. Utilizado para criar senha.
> Guardar senhas mentalmente, cofre digitais.
> Use senha de 8 caracteres.

- lastlog: ùltimos dados do log.
- last: Dados de entrada e saída.
- logname: nome do usuário atual.
- id: Mostra os grupos do usuário.
- cat/etc/passwd: toda todos os usuários.
- userdel -r: deleta a pasta pessoal do usuário.

## Grupos

Permitem organizar os usuários e definir as permissões de acesso de arquivos e diretórios de forma mais fácil.

cat/etc/group - mostra todos os grupos do sistema.

group - mostra todosos grupos do usuário.

addgroup - cria um grupo.

adduser e gpasswd -a - adiciona um usuário ao um grupo.

gpasswd -a - remove um usuário de um grupo.

groupdel - remove um grupo.

**Lembrando "grep" você pode procura qualquer coisa pelo linux.**

## Permissões

em arquivos e diretórios servem para restringir acessos como: leitura, escritas e execução.
-r
-w
-x

ls -lh:

dono | grupo | outros

chmod: muda a permissão de um arquivo ou diretório.

## Modelo Octal

 User(owner) | Group       | Other       |
 ------------|-------------|-------------|
  R  | W | X |  R  | W | X |  R  | W | X |
  4  | 2 | 1 |  4  | 2 | 1 |  4  | 2 | 1 |

cdmod 777 - Recebe todas as permissões!!