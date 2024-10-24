# Classificação de Pessoas da Turma com Redes Neurais Convolucionais (CNN)

Este projeto utiliza **Redes Neurais Convolucionais (CNN)** para realizar a classificação das pessoas com base em imagens de suas faces. As imagens são coletadas e organizadas em um dataset, treinadas no Google Colab, e depois testadas em tempo real ou utilizando uma imagem estática em .jpg.

## Descrição do Projeto

O objetivo é classificar corretamente faces com base em um modelo de CNN treinado com imagens de cada pessoa. Aproximadamente 200 imagens (ou mais para melhor classificação) são coletadas usando uma webcam e organizadas em pastas com os nomes das clases(pessoas). As possíveis aplicações incluem:
- **Reconhecimento facial** em grupos ou equipes;
- **Segurança e autenticação**;
- **Classificação personalizada** em ambientes educacionais ou eventos.

## Instruções de Instalação

### a) Arquivos Necessários
1. **Teachable Machine**: Utilize para gerar as pastas de classificação das faces. Cada pessoa deve tirar cerca de 200 imagens com sua webcam e baixar a pasta referente ao seu nome em "Download Samples".
2. **Google Colab**: Para realizar o treinamento completo da CNN. O dataset gerado deve ser carregado no Colab em arquivo zipado carregando as classes separadas em pastas.
3. **Irium ou Webcam**: Utilizados para testar o modelo em tempo real após o treinamento.

### b) Salvando os Arquivos
Após o treinamento no **Google Colab**, três arquivos serão gerados:
- **Modelo JSON**: Estrutura do modelo;
- **Modelo H5**: Pesos do modelo;
- **Arquivo TXT**: Classes e índices.

Esses arquivos devem ser salvos localmente junto com o código de teste fornecido. Eles serão utilizados para testes no **Anaconda** ou **VSCode**.

## Instruções de Uso


### a) Treinamento no Google Colab
- Carregue o dataset no **Google Colab** e use o código de treinamento da CNN fornecido. Ajuste os parâmetros conforme necessário:
  - **Tamanho do kernel**
  - **Taxa de aprendizado**
  - **Batch-size**
  - **Quantidade de épocas**
  - **Quantidade de camadas convolucionais e densas**

### a) Testando no Anaconda ou VSCode
Para realizar o teste, adicione os três arquivos gerados pelo treinamento (modelo JSON, pesos H5 e classes TXT) em uma pasta, junto com o arquivo de teste, que pode ser para classificação estática de imagens ou usando uma webcam. Execute o arquivo de teste no **Anaconda** ou **VSCode**, e o modelo deverá classificar corretamente as faces capturadas pela webcam ou presentes nas imagens. Caso a classificação não seja precisa, ajuste os parâmetros do modelo, como o número de camadas, tamanho do kernel ou taxa de aprendizado, e treine novamente até obter uma classificação adequada.

## Créditos
Projeto realizado no **Laboratório de Sistemas de Informação da UFOPA**, com contribuições dos alunos da turma. O treinamento da rede neural foi realizado no **Google Colab** e o teste no **Anaconda**, com uso de webcam ou o aplicativo **Irium** para avaliação da disciplina de Processamento de imagens.



