Integrantes: Diego Polanski de Feitas Viera; Guilherme de Almeida Santos; Raphael Arnaut Rossi;

Descrição do Trabalho:

Para atender ao que foi solicitado de reaproveitamento dos espaços vazios, nosso grupo decidiu modificar os métodos Create e Update. Ao invés de apenas adicionar os registros no final, optamos por percorrer o arquivo em busca de espaços vazios. Quando encontramos um espaço vazio com tamanho igual ao registro que desejamos inserir, substituímos esse espaço vazio. Desta forma, conseguimos minimizar os casos de desperdício de espaço. No melhor caso, o arquivo não teria nenhum espaço vazio.

Durante o processo, o mais desafiador foi pensar em como lidar com cada detalhe dos espaços vazios que surgem. Ao deletar ou atualizar um registro, muitas vezes surgem espaços vazios. Para abordar isso, pensamos na estratégia de percorrer o arquivo em busca de registros deletados, a fim de reutilizar esses espaços. Conseguimos alcançar nossos objetivos, produzindo um código organizado, com sentido e comentado. Além disso, adicionamos um menu com opções para Criar, Ler, Deletar e Atualizar, simulando um CRUD de um sistema real. Em cada etapa do processo, uma instrução é fornecida para evitar erros na execução. Não são permitidos valores incompatíveis, sendo que o programa alerta e solicita correções quando necessário. Ao final da função main, adicionamos um conjunto de testes que exemplifica cada caso: criar no final, criar usando um espaço vazio, atualizar no final, atualizar usando um espaço vazio e atualizar no local do registro original. Foi um trabalho divertido de realizar, onde aprimoramos nossos conhecimentos na manipulação de dados em arquivos de bytes.


Checklist:
* Qual foi considerada uma perda aceitável para o reuso de espaços vazios, isto é, quais são os critérios para a gestão dos espaços vazios?
   - No nosso melhor caso, a perda é zero. No entanto, consideramos aceitável um espaço vazio que não corresponda ao tamanho de nenhum registro ou atualização.

* O código do CRUD com arquivos de tipos genéricos está funcionando corretamente?
   - Sim, está funcionando perfeitamente.

* O CRUD tem um índice direto implementado com a tabela hash extensível?
   - Não.

* A operação de inclusão busca o espaço vazio mais adequado para o novo registro antes de acrescentá-lo ao fim do arquivo?
   - Sim.

* A operação de alteração busca o espaço vazio mais adequado para o registro quando ele cresce de tamanho antes de acrescentá-lo ao fim do arquivo?
   - Sim.
     
* As operações de alteração (quando necessário) e de exclusão estão gerenciando os espaços vazios para que possam ser reaproveitados?
   - Sim.

* O trabalho está funcionando corretamente?
   - Sim.
     
* O trabalho está completo?
   - Sim.

* O trabalho é original e não uma cópia do trabalho de um colega?
   -Trabalho original.
