# Análise de Preços de Imóveis com Machine Learning

> **Automatiza a previsão de preços de imóveis utilizando modelos de Machine Learning e uma interface de Streamlit para interatividade com o usuário.**

## 🚀 Tecnologias e Bibliotecas Utilizadas

- **Python**: Python 3.12.1.
- **Pandas**: Para manipulação e análise de dados.
- **Streamlit**: Para criar uma interface web interativa para previsão de preços.
- **Joblib**: Para salvar e carregar o modelo treinado.
- **NumPy**: Para operações matemáticas e manipulação de arrays.
- **Seaborn/Matplotlib**: Para visualização de dados e gráficos.

## 📋 Funcionalidades:

- **Interface Streamlit**: Permite ao usuário inserir informações sobre imóveis, como localização, características e políticas de cancelamento, para prever o preço.
- **Processamento de Dados**: Converte entradas em variáveis numéricas e categóricas para alimentar o modelo treinado.
- **Previsão de Preços**: Utiliza um modelo treinado (Extra Trees Regressor) para prever o preço do imóvel com base nas informações fornecidas. O Extra Trees Regressor foi escolhido por proporcionar um alto R² (97.53%) e um baixo RSME (41.69), garantindo precisão e eficiência na previsão.
- **Envio de Resultado**: Exibe o preço estimado do imóvel na interface.

## 📂 Estrutura do Projeto

```plaintext
├── machine-learning/   # Diretório principal contendo scripts e arquivos necessários
    ├── dataset/                       # Diretório para arquivos utilizados para treinamento e teste.
    ├── main.ipynb                     # Notebook principal com a lógica do modelo de previsão.
    ├── description.ipynb              # Notebook com toda a descrição do projeto.
    ├── requirements.txt               # Dependências do projeto.
    ├── model.joblib                   # Modelo treinado salvo.
    ├── deploy.py                      # Script de deploy para execução do modelo de previsão com Streamlit para simulação com dados reais.
    ├── dados.csv                      # CSV criado a partir do nosso MAIN script para auxílio no projeto.
    ├── primeiros_registros.csv        # CSV criado a partir do nosso MAIN script para auxílio no projeto.
    └── README.md                      # Este arquivo.
```

## ⚠️ Informações IMPORTANTES

- **Faça o download da base de dados no link abaixo e salve na pasta "dataset" dentro do projeto antes de executar qualquer ação**: [Base de Dados Airbnb Rio de Janeiro](https://www.kaggle.com/allanbruno/airbnb-rio-de-janeiro)

- **Devido ao tamanho do arquivo final do modelo já processado, não é possível disponibilizá-lo no GitHub. Portanto, execute o código para gerar o seu próprio `model.joblib` e mantenha-o sempre na pasta RAIZ do projeto.**

## 💾 Instruções para Executar o Deploy.py

- **Instale as Dependências**: Certifique-se de ter o Python e as bibliotecas necessárias instaladas. Você pode instalar as dependências utilizando o seguinte comando no terminal:

```plaintext
pip install -r requirements.txt
```

- **Executando o deploy.py**: Navegue até o diretório onde está localizado o arquivo Deploy.py e execute no terminal o comando abaixo:

```plaintext
python deploy.py

ou

streamlit run Deploy.py
```

- **Interface Streamlit**: Após a execução, a interface do Streamlit estará disponível no seu navegador. Basta acessar o link mostrado no terminal para interagir com o modelo. 🌐

## ✨ Author

- Name: Kauan Gouveia Cipullo.
- LinkedIn: https://www.linkedin.com/in/kauan-cipullo/
- Email: kaauan_@hotmail.com
