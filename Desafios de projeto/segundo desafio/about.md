Nesse projeto, trabalhamos o processamento e transformação de dados com a ferramenta PowerBI. O dataset utilizado origina de uma Base de Dados SQL e foi integrado através da Azure, cujo script pode ser encontrado no Módulo 3 deste repositório, mas tambem incluí os arquivos JavaScript Object Notation gerados no phpMyAdmin. Foram aplicadas as etapas (abaixo) indicadas no desafio com o PowerQuery e, por fim, foi criado um breve relatório no PowerBI.

1. Verifique os cabeçalhos e tipos de dados
2. Modifique os valores monetários para o tipo double preciso
3. Verifique a existência dos nulos e analise a remoção
4. Os employees com nulos em Super_ssn podem ser os gerentes. Verifique se há algum colaborador sem gerente
5. Verifique se há algum departamento sem gerente
6. Se houver departamento sem gerente, suponha que você possui os dados e preencha as lacunas
7. Verifique o número de horas dos projetos
8. Separar colunas complexas
9. Mesclar consultas employee e departament para criar uma tabela employee com o nome dos departamentos associados aos colaboradores. A mescla terá como base a tabela employee. Fique atento, essa informação influencia no tipo de junção
10. Neste processo elimine as colunas desnecessárias.
11. Realize a junção dos colaboradores e respectivos nomes dos gerentes . Isso pode ser feito com consulta SQL ou pela mescla de tabelas com Power BI. Caso utilize SQL, especifique no README a query utilizada no processo.
12. Mescle as colunas de Nome e Sobrenome para ter apenas uma coluna definindo os nomes dos colaboradores
13. Mescle os nomes de departamentos e localização. Isso fará que cada combinação departamento-local seja único. Isso irá auxiliar na criação do modelo estrela em um módulo futuro.
14. Explique por que, neste caso supracitado, podemos apenas utilizar o mesclar e não o atribuir.
    Ambas as operações são utilizadas na combinação de dados de diferentes fontes ou tabelas. Elas diferem no sentido em que Mesclar (Merge) utiliza de uma chave de mesclagem, ou seja uma coluna em comum entre as tabelas, assim como funciona a operação `JOIN` e seus subtipos no SQL. Atribuir (Append) empilha as linhas de uma tabela em cima da outra, exigindo que as tabelas envolvidas possuam a mesma estrutura de colunas.

15. Agrupe os dados a fim de saber quantos colaboradores existem por gerente
16. Elimine as colunas desnecessárias, que não serão usadas no relatório, de cada tabela
