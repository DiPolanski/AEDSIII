TP 2 – Busca por Palavras

Grupo: Diego Polanski, Guilherme de Almeida e Raphael Arnault

Durante a execução do projeto, começamos adaptando a pesquisa para ocorrer não apenas pelo ID, mas também pelo título e autor. Após sucesso nesse processo, decidimos aprimorar a busca, implementando a funcionalidade de divisão das palavras para uma busca mais abrangente.

A parte mais desafiadora do projeto foi lidar com os IDs duplicados que surgiam dependendo da busca. Para resolver isso, optamos por transformar a lista em uma tabela hash padrão, eliminando os itens duplicados.

Todos os objetivos foram alcançados e o código foi organizado de forma clara e eficiente.

Para executar o trabalho, foi necessário modificar todas as etapas do CRUD.

Criamos uma função para realizar o "split" do título e dos autores dos livros, retornando um array de strings com a divisão da frase.
Create:
Após o usuário preencher todos os dados do registro, realizamos o "split" para o título e o autor.
Em seguida, cada palavra do array de strings foi adicionada à lista invertida por meio de um laço de repetição.
Criamos duas listas invertidas, uma para os títulos e outra para os autores.
Read:
No momento da leitura, disponibilizamos duas opções para o usuário: pesquisar pelo título ou pelo autor.
Após a escolha, a string é coletada e enviada para uma função de leitura específica para cada modelo de busca.
A string é então processada pela função de "split".
O resultado é enviado para uma função que cria um array com todos os IDs correspondentes à busca nas listas invertidas (tratando para evitar IDs duplicados).
Cada ID desse array é enviado ao método read original, que busca o registro.
Por fim, os dados de todos os registros que correspondem à busca são exibidos na tela.
Update:
Ao selecionar o "update", o usuário escolhe qual ID será atualizado.
Em seguida, escolhe qual item será atualizado (título, autor ou preço) e insere o novo valor.
O valor antigo é armazenado para ser removido da lista.
O novo valor é registrado na lista.
Delete:
O usuário informa qual ID deseja deletar.
O título e o autor desse registro são armazenados.
Os dados correspondentes ao ID inserido pelo usuário são removidos das listas.
Observações:
Todas as palavras são transformadas em minúsculas nas listas invertidas, durante a pesquisa e as atualizações, garantindo que as operações ocorram corretamente, independentemente da forma como foram escritas.
As stop words e palavras com menos de 4 letras foram removidas de todo o processo.
Os autores foram incluídos nos registros, além do mínimo exigido.
Questionário

Sim, cada termo do título e do nome do autor é acrescentado.
Sim, todas as atualizações são refletidas na lista, removendo a relação do antigo nome com o ID atualizado e criando a relação com o novo título.
Sim, todo registro apagado resulta na remoção correspondente na lista.
Sim, as stop words foram removidas do processo, assim como palavras com menos de 4 letras.
Além do mínimo, os autores foram incluídos nos registros.
Todas as funções estão operando corretamente.
O trabalho está completo com todos os requisitos necessários.
O trabalho é original.
