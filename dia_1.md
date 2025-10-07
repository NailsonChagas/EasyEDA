Projeto do circuito eletronico não será aborado nesse curso

Etapas do curso:
1. Esquematico do circuito no EasyEDA
2. Fazer as routes (rotas) da PCB
3. Confecção da placa (transferencia termica + corrosão)
4. Montagem e teste

Da etapa 1 para 2 é importante checar o DRC (Menu design)

Conceitos importantes:
- footprint -> como o componente fica da placa
    - SOP
    - SO
    - PDIP
    - DIP
    - SOIC
- th -> through-hole -> furado (que tem que usar socket ou furar a placa) 
- smd -> Surface-mount technology -> sentado em cima da placa, menor que th e mais baratos, mas com dificuldade maior de manusear


Circuito a ser montado será um VU meter
- Componentes a serem usados:
    - TL082CP
    - th 

Um esquematico pode ter mais de uma folha, circuitos complexos podem ser divididos para facilitar o desenvolvimento, no curso sera usado uma folha apenas

Comandos importantes:
- P -> place -> abre menu ne inserção de componentes padrões
- P + P -> interface para procura de componentes em forncedores


Na hora de colocar componentes: 
- X.1, X.2 -> mesmo componente X mas em canais diferentes (mesmo ci pode ter mais de um componente)
- Numeros nos componentes indicam qual a porta no componente 