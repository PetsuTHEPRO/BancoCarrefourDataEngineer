# Manipulando Arquivo

O que é Shell Script? Shell em computação é uma interface de usuário para acessar os serviços de um sistema operacional.
  
Script é uma linguagem de programação que executa no sistema em tempo de execução, muito utilizado para automação.

## CD - Muda de Diretório

Esse acrônimo é devido ao sistama de antigamentoe não terem muita memória.

cd - é acrônimo da expressão inglesa (change directory).

Algumas derivações:  

Comandos | Funções |
---------|---------|
cd /     | Abre o diretório raiz do sistema|
cd ~     | Abre o diretório do usuário corrente, o usuário logado naquele instante. |
cd ..    | Para volta um diretório |

## LS - Listando Arquivos

Algumas derivações

Comandos|funções|
----|-----|
ls -l| Lista o conteúdo em coluna detalhada.|
ls -a| Lista o conteúdo até os arquivos ocultos.|
ls -s | Lista o conteúdo com tamanho alocado de cada arquivo, em bloco. |

## TOUCH - Criar e Atualizar o Conteúdo

Usado para criar arquivos vázios.

formatos:

- Para criar dois arquivos ao mesmo tempo: touch "NomeArquivo1"."extensão" "NomeArquivo2"."extensão" ...
- Alterar Hora de Acesso: touch -a "NomeArquivo"."extensão"
- Alterar Hora de Modificação: touch -m "NomeArquivo"."extensão"
- Alterar Hora de Acesso sem criar um novo arquivo: touch -c "NomeArquivo"."extensão"
- Definir Hora Específica de Acesso e Modificação: touch -t CCYYMMDDhhmm.ss "NomeArquivo"."extensão"

## CAT - Visualizar conteúdo do arquivo

Cat - Concatenar

- Criar arquivos.
- Unir arquivos.
- Exibir arquivos.

## Lembrete

> Redicionador de saída: ">"

## MV - Mover e Renomear Arquivos

Use as Flags:

- -i: Confirme antes de substituir.
- -n: Sem substituição.
- -b: Substituição pelo backup.
- -u: Substituía se o arquivo de destino for antigo ou não existir.

## CP - Copiar Arquivos

Use as Flags:

- -i: Confirmação antes de substituir.
- -v: Mostra a saída do processo da copia.

## MKDIR - Cria Diretório

## RM - Remove Arquivos

- rm: Remove o arquivo.
- rm -f: Força a remoção do arquivo.

## Find - Procura arquivo

find ./ -type (f,d) -name "o": Mostra todos os arquivos com a letra "O".

## RMDIR e RM -RF - Remove Diretório

Para remover diretório vazio rmdir "Nome do diretório"
Para remover diretório cheio rm -rf "Nome do diretório"

# Variável de Ambiente

env: Variáveis de Ambiente.

PSD1: Prompt da linha de comandos.
HOME: Diretório "/home" de um usuário;
PATH: Lista de diretórios vasculhandos quando um comando é executado.

Para criar ("Variavel"="valor")

**export** para transferir para variáveis de ambiente.