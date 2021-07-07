# Mentoria #1

Professor: Marcos Roberto.

"Conhecimento bom é aquele compartilhado." ~ Marcos Roberto.

Professor: Bruno Arthur, Banco Carrefour.

- Onde o linux entra nessa área de dados.

Dicas: 

- Para aprender linux, sai da zona de conforto. Trazer por meu dia-a-dia.
- Ter uma base teórica é perfeito, mas fazer é melhor ainda. (Errar é aprender)

"O dado ele nasce de um lugar, deve ser trabalhado e vai ser armazenado."

Mas onde o shell entra nesse cenário.

- pwd: mostra o caminho atual
- ls: mostra os diretórios (-lhtr)

"Organização é muito importante, principalmente com arquivos muito extensos."
"Use atalhos(Tab) para melhorar a agilidade."
"Use o vi no linux"

> Código SHELL Abordado na Aula

```
cd /home/au_929001077/LIVEDIO/Sources/ ;

MASCARA=AcqFeed_madresslinks;

echo 1 > ${MASCARA}_err.log;

QTD=`echo ${MASCARA} | wc -c`;

echo 2 >> ${MASCARA}_err.log;

#Qts de caracteres da prefixo + lote + mascara$
QTD_INIT= `echo 24+QTD | bc `;

echo 3 >> ${MASCARA}_err.log;

#Qts de caracteres da prefixo + mascara + data$
QTD_FIM=`echo 7+$QTD_INIT | bc` ;

echo 4 >> ${MASCARA}_err.log;

DATA=`ls -tr R06_??????_BR_DWH_${MASCARA}_????_*_*_*.txt | head -1 | cut 
-c${QTD_INIT}-${QTD_FIM}` ;

status=$?;

echo status a = $status >> ${MASCARA}_err.log;

echo 5 >> ${MASCARA}_err.log 2>&1 ;

echo 6 >> ${MASCARA}_err.log;


ls -tr R06_??????_BR_DWH_${MASCARA}_????_${DATA}_*_*.txt > Arq_Lista_${MASCARA}.txt;

echo 7 >> ${MASCARA}_err.log;

status=$?;

echo status b = $status >> ${MASCARA}_err.log;

echo 8 >> ${MASCARA}_err.log

echo [ODS_TSYS.WF:wf_D_TODS_TSYS_$MASCARA] >> Arq_CTL_${MASCARA}.txt;

echo \$DBConnection_ODS=BI_ODS >> Arq_CTL_${MASCARA}.txt;
echo \$DBConnection_STG=BI_STG >> Arq_CTL_${MASCARA}.txt;
echo \$\$REFDATE=$DATA >> Arq_CTL_${MASCARA}.txt;

#rm ${MASCARA}_err.log;

```

> Coloque um comando entre ` ` para imprimir o resultado do comando.
use o "sh" para executar arquivos shell.
