# abntex IFPI
Modificações ao ABNTeX para TCCs do IFPI.

Este projeto contém uma série de modificações e ajustes ao modelo ABNTeX original as quais o adaptam para os padrões exigidos pelo IFPI.

## Como Usar
Primeiro altere os arquivos na pasta `este-trabalho`. Lá estão todos os meta-dados sobre o TCC como título, orientador, membros da banca examinadora, resumo e abstract, dedicatória, etc.

A maioria dos arquivos tem nomes auto explicativos. Comece vendo e modificando o arquivo `este-trabalho\informacoes.tex`. Depois, na mesma pasta, veja `este-trabalho\resumo-abstract.tex`, por exemplo.

Após configurar as informações de seu trabalho, há mais duas coisas a fazer.

## Adicionando capítulos
Na pasta `capitulos` ficarão os arquivos que farão a parte textual de seu trabalho. Cada arquivo `.tex` representa um capítulo completo. Se você tiver conhecimentos mais avançados de TeX sinta-se livre para criar uma estrutura de arquivos como preferir.

Para **adicionar** um capítulo no TCC você deve:

1. Criar um arquivo para o capítulo. Neste exemplo, vamos criar `capitulos\exemplo.tex`.
2. Adicioná-lo em `capitulos\capitulos-tcc.tex`: `\input{capitulos\exemplo}` (o `.tex` é opcional).

Para **remover** um capítulo basta retirar o `\input{...}` do arquivo `capitulos\capitulos-tcc.tex` (apagando ou comentando).

## Compilando e gerando o TCC
Depois de configurar tudo do projeto e os capítulos basta compilar o arquivo `documento.tex` que está na raiz do projeto.

## O que falta
Ainda não organizamos a inclusão de apêndices que, no momento, deve ser feita manualmente no arquivo `pos-textual\finalizacao.tex`.
