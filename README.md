# Relatório Técnico: Previsão e Conscientização sobre Consumo de Energia

## Descrição do Problema

A otimização do consumo de energia elétrica é uma das maiores preocupações em termos de sustentabilidade. A conscientização e a previsão precisa do consumo de energia são essenciais para o uso eficiente de recursos. Este projeto aborda o problema com duas abordagens:
1. **Educação**: Através de um quiz educativo interativo sobre práticas de consumo energético.
2. **Previsão e Análise**: Usando técnicas de Machine Learning e clusterização para prever o consumo de energia e identificar padrões de uso.

## Metodologia

### 1. Geração de Dados
Os dados são gerados de maneira realista, considerando:
- **Mês**, **feriado**, **temperatura**, **umidade**, **habitantes**, **potência consumida**, e **estação do ano**.
O dataset gerado contém 1000 amostras e é usado para treinar o modelo de Machine Learning e para a análise de clusterização.

### 2. Modelo de Machine Learning
- **Modelo**: Random Forest Regressor
- **Objetivo**: Prever o consumo de energia com base nas variáveis mencionadas.
- **Avaliação**: O modelo é avaliado utilizando o erro absoluto médio (MAE) e o **R²**, que indica a capacidade do modelo de explicar a variabilidade dos dados.

### 3. Clusterização com K-Means
A técnica de clusterização K-Means é aplicada para identificar grupos com padrões semelhantes de consumo de energia com base em variáveis como temperatura, umidade e consumo de energia.

### 4. Quiz Educativo
O quiz educativo contém 8 perguntas sobre consumo de energia, fontes de energia renováveis e não renováveis, e práticas para economizar energia.

### 5. Sistema de Login e Cadastro
Foi implementado um sistema de login e cadastro de usuários para personalizar a experiência. Os dados dos usuários são armazenados em um banco de dados SQLite, permitindo login com credenciais previamente cadastradas.

### 6. Gerenciamento de Dados do Usuário
Após o login, o usuário pode adicionar ou atualizar seu telefone e endereço, além de visualizar esses dados. A função "Voltar ao Quiz" permite que o usuário retorne à parte educativa do projeto, garantindo uma experiência interativa e personalizada.

## Resultados Obtidos

- **Modelo de Previsão**: O Random Forest apresentou uma boa performance, com **R² alto** e **MAE baixo**, indicando que o modelo pode ser eficaz para prever o consumo de energia.
- **Clusterização**: A segmentação dos dados por clusterização mostrou padrões distintos de consumo baseados em variáveis climáticas e de potência consumida.
- **Quiz Educativo**: O quiz ajudou a engajar os usuários, promovendo a conscientização sobre a importância do consumo sustentável de energia.
- **Sistema de Login e Cadastro**: O sistema de login/cadastro foi bem-sucedido em permitir que os usuários salvassem e atualizassem seus dados pessoais, criando um ambiente mais interativo e personalizado.
- **Gerenciamento de Dados**: Os usuários puderam inserir, atualizar e visualizar suas informações de contato, tornando o projeto mais completo e interativo.

## Conclusões

Este projeto demonstrou como a combinação de **Machine Learning** para previsão de consumo de energia com **educação interativa** pode ser eficaz para promover práticas sustentáveis de consumo de energia. A técnica de clusterização também foi útil para entender melhor os padrões de consumo com base em variáveis climáticas e socioeconômicas. Além disso, o sistema de login e o gerenciamento de dados permitem uma experiência personalizada para o usuário.

## Como Executar

1. Instale os pacotes necessários:
   ```bash
   pip install pandas numpy matplotlib scikit-learn
Execute o código Python para gerar o dataset, aplicar o modelo de previsão, a clusterização e o quiz.
Utilize o sistema de login/cadastro para gerenciar seus dados pessoais.
Responda às perguntas do quiz para testar seus conhecimentos sobre o consumo de energia!
Tecnologias Utilizadas
Python 3.x
Bibliotecas:
pandas para manipulação de dados.
numpy para geração de dados aleatórios.
matplotlib para visualização.
scikit-learn para modelagem de machine learning e clusterização.
SQLite para o gerenciamento de dados de usuários (login, cadastro, e dados pessoais).
