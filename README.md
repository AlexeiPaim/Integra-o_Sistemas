# Integracao_Sistemas
Projetos desenvolvidos para a disciplina de  Integração de sistemas para Automação 



BLU3024-09754 (20232) - Integração de Sistemas para Automação
Trabalho prático - Enunciado 5
1. Introdução

Este trabalho tem o objetivo de modelar e popular um banco de dados com informações sobre o histórico escolar de alunos de curso superior.

2. Enunciado

Modelar e implementar um banco de dados relacional que permita armazenar o histórico escolar de alunos de curso superior. Esse histórico consiste das disciplinas cursadas pelos alunos ao longo dos semestres de formação do curso, bem como do aproveitamento obtido pelos alunos e de sua frequência nas disciplinas. Os dados que devem ser armazenados são:

Disciplinas já cursadas pelo aluno. Essa informação deve incluir o código e o nome da disciplina, bem como o semestre letivo em que ela foi cursada, a nota final obtida pelo aluno (entre 0 e 10.0) e a frequência do aluno.
Disciplinas que o aluno ainda deve cursar para concluir sua formação.
Obervações:

Cada aluno é identificado por um código identificador e por um nome.
Cada disciplina tem um código composto por letras e números (ex. BLU3024), um nome, e a fase de formação (1, 2, 3, ...)  em ela que ocorre dentro de cada um dos diferentes cursos. 
Uma disciplina pode ser oferecida a diferentes cursos e pode acontecer em diferentes fases em diferentes cursos. Por exemplo, uma mesma disciplina pode ser oferecida na 2ª fase de um curso e na 4ª fase de outro.
As disciplinas podem ter, como pré-requisitos, outras disciplinas. Para que um aluno possa cursar uma disciplina, ele deve ter sido aprovado nos pré-requisitos, se houverem.
Um aluno é considerado aprovado em uma disciplina quando obtém nota final igual ou superior a 6.0 e frequência igual ou superior a 70%.
Um aluno pode cursar mais de um curso ao mesmo tempo. As disciplinas em que o aluno é aprovado são aproveitadas em todos os cursos em que ela é oferecida e que que o aluno esteja cursando. Por exemplo, se a disciplina Cálculo I é oferecida tanto no curso de Engenharia de Controle e Automação quanto no curso de Engenharia Têxtil, então um aluno que cursa ambos os cursos e que tenha sido aprovado em Cálculo I aproveita os seus créditos em ambos os cursos.
3. Entregas

Trabalho a ser realizado em grupos de 4 elementos.

Importante: informar a formação dos grupos até as 23h59 do dia 17/09/2023 através do item apropriado no Moodle. Assume-se que alunos que não sinalizarem participação em grupo algum não entregarão o trabalho.

Entregar, até o dia 15/10/2023, via Moodle, os seguintes itens:

3.1 Modelos conceitual e lógico. Podem ser entregues arquivos gerados no BrModelo ou em qualquer outro software. No caso de arquivos gerados em softwares diferentes do BrModelo, entregar os modelos em formato pdf ou como imagem (jpeg, png etc).

3.2 Arquivo texto contendo script SQL para a criação das tabelas e para a inserção de registros de exemplo. Incluir tantos registros quantos forem necessários para testar as consultas definidas no item 3.3 deste enunciado.

3.3 Arquivo texto com as seguintes consultas SQL:

Listar todos os alunos cadastrados no banco de dados em ordem de código identificador;
Listar todos os alunos cadastrados no banco de dados em ordem alfabética de nome;
Listar todas as disciplinas de um determinado curso (a ser informado na consulta SQL) ordenadas pela fase em que ocorrem e, como segundo critério, pelo seu código;
Listar os nomes das disciplinas que são oferecidas em mais de um curso;
Listar código e o nome das disciplinas que são pré-requisito para uma determinada disciplina, cujo código deve ser informado na consulta SQL.
Listar o nome de todos os alunos de um determinado curso (a ser informado na consulta SQL) e a média geral obtida por cada um deles. Essa média é a média de todas as notas finais obtidas pelo aluno. A consulta deve ser ordenada de forma decrescente pelas médias gerais dos alunos (alunos com média maior aparecem primeiro).
Listar as disciplinas que um determinado aluno (cujo código deve ser informado na consulta SQL) pode cursar. Estas disciplinas são aquelas que (i) não têm pré-requisito ou (ii) cujos pré-requisitos foram cumpridos;
Listar as disciplinas que requerem a aprovação em apenas um pré-requisito para poderem ser cursadas por um determinado aluno (cujo identificador deve ser informado na consulta SQL).
3.4 Implementação do banco de dados em algum SGBD. A implementação deve estar disponível em uma máquina virtual fornecida pela UFSC (informações aqui), em alguma outra máquina virtual que possa ser acessada pela Internet, ou em uma imagem Docker.

3.5 Documento com informações para acesso à máquina virtual e ao banco de dados implementado do item 3.4.

4. Apresentação

O grupo apresentará o trabalho ao professor a partir da segunda quinzena de outubro de 2023, em data a definir. A apresentação consistirá em:

4.1. discussão sobre os modelos conceitual e lógico;

4.2 execução do banco de dados criado pelo grupo;

4.3 execução de consultas SQL solicitadas pelo professor (sem consulta ao qualquer material).

5. Avaliação:

Item 3.1. Peso: 15%. Os modelos devem refletir corretamente os requisitos do cenário descrito no enunciado, bem como as demais decisões tomadas pelo grupo no projeto do banco de dados. Além disso, devem estar consistentes entre si.
Item 3.2. Peso: 5%. O script deve poder ser executado sem erros, produzindo o schema que permita a execução das consultas solicitadas.
Item 3.3. Peso: 35% As consultas devem retornar resultados corretos. Todas as consultas têm o mesmo peso na avaliação.
Itens 3.4 e 3.5. Peso: 5%. A máquina virtual deve funcionar corretamente a partir dos passos descritos no documento fornecido pelo grupo, sem requerer configurações adicionais.
Item 4.1. Peso: 5%. O grupo deve fornecer respostas consistentes ao professor com respeito aos modelos conceitual e lógico;
Item 4.2. Peso: 5%. O grupo deve ser capaz de colocar o banco de dados em execução;
Item 4.3. Peso: 30%. O grupo deve executar as consultas corretamente.



Última atualização: Wednesday, 11 Oct 2023, 15:59
