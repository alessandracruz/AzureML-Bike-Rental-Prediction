# AzureML Bike Rental Prediction

## Descrição

Este projeto foi desenvolvido como parte do laboratório do curso **Azure AI Fundamentals**. O objetivo era criar um modelo preditivo para prever a quantidade de bicicletas alugadas, utilizando o **Azure Machine Learning Studio**.

------

### Referência

Para acessar o laboratório original que inspirou este projeto, visite o [Laboratório de Machine Learning do Microsoft Learn](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html).

Durante o projeto, foi criado um pipeline completo para treinamento e implantação do modelo, com os seguintes passos:

1. **Criar um Workspace no Azure Machine Learning**:
   Configuração de um espaço de trabalho no Azure para gerenciar os experimentos de aprendizado de máquina.
2. **Usar o aprendizado de máquina automatizado para treinar um modelo**:
   O modelo foi treinado utilizando AutoML, com base nos dados fornecidos no laboratório.
3. **Revisar o melhor modelo**:
   Após o treinamento, o melhor modelo foi revisado e escolhido para implantação.
4. **Implantar e testar o modelo**:
   O modelo foi implantado em um endpoint gerenciado, configurado para consumo online.
5. **Testar o serviço implantado**:
   Durante o teste do serviço implantado, foi identificado um erro de rede (**Network Error**) ao tentar consumir o modelo.
6. **Limpeza (Clean-up)**:
   Como o projeto está em um ambiente de aprendizado, foi mantida a configuração do workspace para futuras revisões, mas os recursos não utilizados foram limpos para evitar custos.

------

## Tecnologias Utilizadas

- **Azure Machine Learning Studio**: Configuração do ambiente, treinamento e implantação do modelo.
- **JSON**: Para entrada e configuração do teste do modelo.
- **Python** (indiretamente no laboratório): Utilizado pelo estúdio do Azure para treinar o modelo.

------

## Estrutura do Repositório

```
bashCopiarEditarAzureML-Bike-Rental-Prediction/
├── README.md               # Documentação do projeto
├── input_config.json       # Arquivo de entrada para teste do modelo
```

- **README.md**: Explicação sobre o projeto, passos seguidos e limitações.
- **input_config.json**: Arquivo JSON gerado pelo Azure Machine Learning Studio, contendo a estrutura necessária para testar o modelo.

------

## Passo a Passo Realizado no Projeto

1. **Criar um Workspace no Azure Machine Learning**:
   - Configurado no Azure para gerenciar o treinamento e a implantação do modelo.
2. **Usar o aprendizado de máquina automatizado para treinar um modelo**:
   - AutoML foi utilizado para selecionar automaticamente o melhor modelo para os dados fornecidos.
3. **Revisar o melhor modelo**:
   - O modelo escolhido foi revisado para verificar métricas e adequação ao problema.
4. **Implantar e testar o modelo**:
   - Implantação feita com sucesso em um endpoint gerenciado, mas os testes enfrentaram problemas de rede.
5. **Testar o serviço implantado**:
   - O teste retornou um erro de rede (**Network Error**) durante o consumo do endpoint.
6. **Limpeza (Clean-up)**:
   - Os recursos desnecessários foram removidos para evitar custos adicionais.

------

- Configuração do Endpoint

  O endpoint criado está configurado conforme a URL e arquivo de configuração abaixo:

  - URL do Endpoint (só como exemplo, pois cada um tem sua própria configuração):

    ```
    https://laboratorioai900-blrhe.eastus.inference.ml.azure.com/score
    ```

  - **Arquivo de Configuração**: O arquivo `input_config.json` contém a estrutura necessária para o envio de dados ao endpoint.

  ------

  ## Observações

  - O endpoint foi configurado e implantado com sucesso, mas não foi possível validar os resultados devido ao erro de rede mencionado.
  - Este projeto pode ser retomado em um momento futuro para investigar e corrigir o problema identificado.

  ------

  ## Como Usar o Arquivo JSON

  1. Copie o conteúdo do arquivo `input_config.json`.
  2. Configure um cliente HTTP com um script em Python para realizar a chamada ao endpoint usando a URL fornecida.
  3. Insira os dados necessários no JSON para realizar o teste.

  ------

  ## Contato

  Se tiver dúvidas ou sugestões, entre em contato:

  - **Nome**: Alessandra Cruz

  - **E-mail**: [alessandraccruz@pm.me](mailto:alessandraccruz@pm.me)

  - **GitHub**: [alessandracruz](https://github.com/alessandracruz)
