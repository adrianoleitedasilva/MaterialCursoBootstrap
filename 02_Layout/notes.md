# Layout

## Inserindo nosso CSS

- O estilo do Bootstrap pode não ser suficiente para finalizar uma aplicação, então podemos trabalhar com um arquivo css nosso.
- Devemos criar o link para o nosso arquivo sempre abaixo da chamada do arquivo do Bootstrap

# Breakpoints

## Introdução

- São pontos específicos de resolução, criados através de media query para deixar o site responsivo
- Eles seguem um padrão que é encontrado na maioria dos dispositivos
- Ou seja, temos um breakpoint para tablet e outro para celular
- Não há para todos, mas para os mais utilizados
- Lembrando que é utilizado um padrão mobile first, ou seja, estilização de menor resolução para a maior.

## Breakpoints do Bootstrap

- Breakpoints do Bootstrap são utilizados por classes como: sm, md, lg
- Cada um representa um media query
- Então normalmente adequamos outros elementos do nosso site a estes breakpoints
- Assim é possível trabalhar com conjunto de Bootstrap e deixar nosso site amigável/responsivo

# Containers

- São entidades importantes do Bootstrap
- Estruturam o layout
- E como o próprio nome diz, são depósitos de outros elementos
- Tempos tipos diferentes de containers

# Container Fluid

- O container fluid utiliza uma área maior para abrigar os elementos
- Sempre representa 100% da área útil
- Eliminando as margens laterais
- A classe é a container-fluid

# Container por Breakpoint

- Podemos também moldar um container por breakpoint
- Utilizamos a classe container-x
- Onde x pode ser: sm, md, lg e outras muitas opções
- Com esta versão, queremos que o container respeite uma largura máxima, que se baseia na resolução.

# Grid

- Grid é uma estrutura para criar layouts em Bootstrap
- Temos um grid colunar, dividido por 12 colunas
- A estrutura do Grid é sempre: container, row, columns
- Onde temos o container para abrigar a seção
- Row para determinar uma linha, largura de 100%
- Columns para subdividir o container em até 12 partes

## Tamanhos das Colunas

- Podemos ajustar o tamanho das colunas
- Para ocupar três espaços: col-3
- Lembrando que podemos separar em no máximo 12 divisões
- E o espaço ocupado será proporcional, ou seja, col-11 e col-1.

## Limitando número de colunas

- Podemos limitar a quantidade de colunas em uma row
- A classe a ser utilizada é a row-cols-x
- Onde x é o limite
- Assim o grid sempre vai respeitar este número máximo NA Linha

## Alinhamento Vertical

- As colunas dentro de uma row estão condicionadas ao flex box
- Ou seja, temos classes bem parecidas com as regras de flex para alinhá-las
- Exemplo: align-items-end, alinhando no fim da row
- Lembrando que esta classe sempre deve ficar no elemento pai, ou seja, na row

## Alinhamento Horizontal

- O alinhamento horizontal segue a mesma premissa do vertical
- Utilizamos classes no elemento pai(row) para condicionar os itens na linha horizontal
- Para centralizar elementos podemos pôr a classe: justify-content-center
- As regras end e start também funcionam
Podemos combinar os alinhamentos vertical e horizontal

## Alinhamento de Itens

- O alinhamento de item serve para alinharmos itens de forma individual
- Utilizamos classes como: align-self-center
- Que alinha um elemento na vertical
- Não há alinhamento unitário para a horizontal

## Ordem dos Items

- É possível alterar a ordem que os itens são exibidos
- Vamos colocar a class order-*
- Onde o * é a posição do elemento, sendo 1 o primeiro
- Este recurso é útil no desenvolvimento mobile, onde os elementos costuma mudar de ordem

## Offset das Colunas

- Podemos criar um espaçamento com o offset
- Ou seja, teremos uma margem da borda definida por uma quantidade de colunas
- Exemplo - offset-md-3
- Neste caso temos um offset de 3 coluna a esquerda

## Gutter

- Os gutters são intervalos que podemos inserir entre as colunas
- É possível inserir no eixo X e Y
- Horizontal = gx-2
- Vertical - gy-4
- Os números que utiulizamos são baseados em rem da página, fonte do elemento root
- O número 3 é a referência para 1rem

Gutter X controla o padding para espaçar o elemento
Gutter Y controla a Margin, que no nosso exemplo está sendo Zerada!