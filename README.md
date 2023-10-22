# Projeto-DIO-Processando-e-Transformando-Dados-com-PowerBI
Projeto DIO sobre o desafio de processamento e transformação de dados utilizando Azure, MySQL Workspace e Power BI para confecção de relatório.

## Passo a passo das mudanças realizadas:
Foram removidas todas as colunas de meta dados de todas as tabelas carregadas.

Verificado todos os cabeçalhos e data types das colunas das tabelas e alteradas caso necessário.

Verificado todos os dados importados, sem necessidade de correção.

Separado coluna complexa de endereço, separando entre endereço, cidade e estado possibilitando uma análise mais detalhada da residência de cada empregado.

Mesclado as tabelas de employee e department para uma tabela nova para a melhor visualização da separação por departamento para cada empregado, removendo colunas desnecessárias para essa análise e renomeando cabeçalhos conforme necessário.

Nessa caso foi utilizado a mescla de tabelas ao invés da combinação, pois a mescla é ação análoga aos ‘joins’ da linguagem SQL, possibilitando uma junção de tabelas diferentes em dados em comum presente em ambas, como nesse caso o número do departamento descrito nas duas tabelas. Em contrapartida, a combinação apenas seria viável em um caso em que as tabelas a serem combinadas possuirem a mesma estrutura de dados em todas as suas colunas, ocasionando nesse caso uma adição de todas as informações como novas linhas na mesma estrutura das tabelas anteriores.

Mesclado a tabela employee consigo mesma, comparando a coluna SSN com Manager SSN em uma junção interna, para a comparação facilitada do nome de cada empregado com o seu gerente. Ao final foi mesclado as colunas de nomes separadas para apenas uma com o nome completo, para os dois casos, e removido colunas desnecessárias.

Mesclado as tabelas de department e dept_locations para facilitar a visualização das diferentes filiais existentes, seguida pela remoção, mescla e renomeação das colunas conforme o necessário. Nesse caso, assim como explicado anteriormente, a combinação das tabelas não seria possível devido à diferença da estrutura das tabelas envolvidas.

Por final foi feito um relatório simples para validar a obtenção correta dos dados trabalhados, apresentado no print abaixo.

![image](https://github.com/guilhermebtatim/Projeto-DIO-Processando-e-Transformando-Dados-com-PowerBI/assets/113799643/e2584b9c-2c45-459d-84c1-4ee97792d819)
