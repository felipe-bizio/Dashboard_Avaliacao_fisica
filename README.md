# Business Case - Dashboard de Acompanhamento de Alunos

## 1. Visão Geral do Projeto:

Este projeto foi desenvolvido com o objetivo de criar uma solução de acompanhamento eficiente e visualmente informativa para um personal trainer, facilitando a análise dos dados de desempenho e evolução física dos alunos. A ferramenta permite tanto o acompanhamento individualizado de cada aluno quanto uma visão geral das atividades e estatísticas da base de alunos. O projeto foi implementado utilizando o Power BI, proporcionando uma interface intuitiva para a análise de dados e relatórios.

## 2. Objetivo do Projeto:

O principal objetivo do dashboard é melhorar a visualização e o acompanhamento das avaliações físicas realizadas com os alunos, permitindo ao personal trainer um acesso rápido a informações detalhadas e uma análise visual clara da evolução física de cada aluno ao longo do tempo. Além disso, ele centraliza informações administrativas relevantes para o controle das atividades do professor.

## 3. Escopo do Projeto:

O dashboard é composto por duas páginas principais:

### Página 1: Relatório dos Alunos
- Filtros de alunos e datas das avaliações.
- Índice de Massa Corporal (IMC)
- Valor do RCQ (Razão Cintura-Quadril)
- Percentual de gordura corporal, calculado pelo método Pollack de 7 dobras.
- Altura, peso e idade.
- Foto do aluno e diagrama do corpo humano com medidas corporais.
- Gráficos de linha que mostram a evolução do peso, percentual de gordura e medidas corporais ao longo do tempo.

### Página 2: Informações do Professor
- Resumo de informações relevantes para o personal trainer, como:
- Número total de alunos.
- Quantidade de avaliações realizadas.
- Distribuição de alunos por gênero.
- Tabelas detalhadas com os dados disponíveis na base de dados.

## 4. Benefícios do Projeto:

- Eficiência na Análise de Dados: O dashboard permite ao personal trainer analisar de forma rápida e precisa a evolução de seus alunos, com informações detalhadas e visualizações claras, otimizando o tempo gasto em análises manuais.
- Acompanhamento Individualizado: A personalização dos filtros permite que o professor visualize a evolução de cada aluno de forma detalhada, facilitando ajustes nos planos de treino e na orientação nutricional com base no desempenho real.
- Centralização de Informações: Todas as informações relevantes dos alunos e do personal trainer estão centralizadas em um único dashboard, facilitando o acesso a dados e a tomada de decisões.

## 5. Solução Técnica:

O projeto foi desenvolvido utilizando o Power BI, uma ferramenta poderosa de visualização e análise de dados. Além de explorar os recursos visuais da plataforma, foram utilizados códigos DAX para a extração e cálculo das medidas, incluindo a fórmula de cálculo da gordura corporal baseada no método Pollack de 7 dobras.

Método Pollack de 7 Dobras: Este método é amplamente utilizado para calcular o percentual de gordura corporal com base na espessura da pele em sete pontos específicos do corpo: peitoral, abdominal, coxa, axilar média, supra-ilíaca, subescapular e tríceps. Esses valores são somados e, a partir de fórmulas específicas para homens e mulheres, o percentual de gordura é calculado. O uso de DAX permitiu automatizar esses cálculos no dashboard, proporcionando resultados instantâneos e precisos conforme os dados das dobras cutâneas são inseridos.

A interface visual foi desenhada de maneira simples e objetiva, visando fácil compreensão e usabilidade para o personal trainer. O uso do DAX garantiu precisão nos cálculos e flexibilidade para atualizações em tempo real com base nos dados das avaliações.

## 6. Próximos Passos:

Projeto ainda em andamento, atualmente em fase de adicionar um chatbot via What'sAPP onde por ele podemos adicionar o cadastro do aluno e alimentar a planilha principal com os dados coletados dos alunos. Por exemplo, ao enviar uma mensagem para o Chatbot, irá retornar uma resposta perguntando se o usuario deseja **"cadastrar um novo aluno"** ou **"adicionar uma nova avaliação"**. Ao selecionar **"cadastrar um novo aluno"**, uma nova mensagem solicitando os dados principais irá aparecer, e após todos os dados serem preenchidos, ele irá armazenar no dataset em uma planilha no google sheets. Ao selecionar a mensagem **"adicionar uma nova avaliação"**, será informado ao usuário uma lista com os nomes de todos os alunos. Ao selecionar um aluno, o chatbot irá solicitar as medidas de circunferencia e posteriormente as medidas das dobras cutaneas. Após totalmente preenchido, os dados serão migrados automaticamente para o dataset e já podem ser avaliados no Dashboard no Power BI.
O projeto será disponibilizado no GitHub como parte de um portfólio profissional, destacando as habilidades em criação de dashboards e visualização de dados no Power BI, com foco em soluções personalizadas para necessidades específicas de clientes.
