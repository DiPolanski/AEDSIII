Integrantes: 
Diego Polanski de Feitas Viera
Guilherme de Almeida Santos
Raphael Arnaut Rossi

Descrição do Trabalho: Para atender com ao que foi pedido, de reaproveitar os espaços vazios, nosso grupo decidiu fazer uma mudança nos métodos Create e Uptade. 
Onde ao invés de apenas adicionarmos os registros no final, iriamos percorrer o arquivo procurando um espaço vazio, e ao acharmos um, com tamanho igual ao registro que vamos inserir, 
sobre escrevemos o local vazio. Dessa forma conseguimos tirar muitos casos de desperdício de espaço. No melhor caso, o arquivo não teria nehum espaço vazio.

Durante o processo, o mais difícil foi pensar como tratar cada detalhe de espaço vazio que surge. Já que quando deletamos ou atualizamos algum registro, muitas vezes surgiram espaços vazio. 
Pensando nisso, pensamos na estratégia de percorrer o arquivo atrás dos registross deletados, a fim de criar ou atualizar os objetos. 
Nós alcançamos o que esperávamos, fizemos um código organizado, com sentido, comentado e adicionamos um menu, para com as opções de Criar, Ler, Deletar e Atualizar. O menu é uma simulação
como se fosse um CRUD de um sistema real. Colocamos como comentario, no final da main. Um caso teste que exemplifica cada caso. Create no final, create usando um espaço vazio, uptade no final, uptade 
usando espaço vazio e uptade no local do registro original.
Foi um trabalho divertido de se fazer, onde conhecemos cada vez mais a manipulação de dados em um arquivo de bytes.


Checklist
* O que você considerou como perda aceitável para o reuso de espaços vazios, isto é, quais são os critérios para a gestão dos espaços vazios?
    No nosso melhor caso a perda é zero, porém temos perda aceitavel um espaço vazio que não condiz com o tamanho de nenhum registro ou atualização.
* O código do CRUD com arquivos de tipos genéricos está funcionando corretamente?
    Está funcionando perfeitamente.
* O CRUD tem um índice direto implementado com a tabela hash extensível?
    Não
* A operação de inclusão busca o espaço vazio mais adequado para o novo registro antes de acrescentá-lo ao fim do arquivo?
    Sim
* A operação de alteração busca o espaço vazio mais adequado para o registro quando ele cresce de tamanho antes de acrescentá-lo ao fim do arquivo?
    Sim
* As operações de alteração (quando for o caso) e de exclusão estão gerenciando os espaços vazios para que possam ser reaproveitados?
    Sim
* O trabalho está funcionando corretamente?
    Sim
* O trabalho está completo?
    Sim
* O trabalho é original e não a cópia de um trabalho de um colega?
    Trabalho original.
