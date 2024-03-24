<body>
<h1 align="center"> CLASSIFICAÇÃO DE IMAGENS 📸 </h1>
<div>
  <p align="center">
        <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/> 
        <img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white"/>  
        <img src="https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white"/><br>
        <img src="https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white"/> 
        <img src="https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black"/>  <br><br>
        <img src='https://github.com/ViniciusSilveiraCampos/Classificador-De-Imagens/assets/108243297/7025c90b-3764-4e09-91e1-9f09877d793e' width="473.5px" height="308.5px"  >

  #

<p align="center">
O projeto de Classificador de Imagens com Rede Neural Convolucional. Com tecnica de aprendizado profundo na análise e classificação de imagens digitais. Utilizando uma arquitetura de rede neural convolucional (CNN), este projeto visa desenvolver um modelo capaz de reconhecer e categorizar imagens em diferentes classes com alto grau de precisão e eficiência.
<br>
<br>


<div>
  <h2 align="left" style="font-size: 24px"> DADOS 📊 </h2>
  <h3 align="left" > Conjunto de Dados CIFAR-100 </h3>
<p align="justify">
O conjunto de dados CIFAR-100 é uma versão do conjunto de dados CIFAR (Conjunto de Dados de Reconhecimento de Imagem Canadense) e é composto por 60.000 imagens coloridas de 32x32 pixels em 100 classes diferentes. Cada imagem pertence a uma das 100 classes, que são divididas em 20 superclasses. Cada classe contém 500 imagens de treinamento e 100 imagens de teste.

### **Classes**

As 100 classes do CIFAR-100 abrangem uma ampla variedade de objetos e cenas do mundo real. Algumas das classes incluídas são:

- Animais (por exemplo, gato, cachorro, cervo, pássaro)
- Meios de transporte (por exemplo, avião, carro, trem, navio)
- Frutas e vegetais (por exemplo, maçã, laranja, morango, cogumelo)
- Instrumentos musicais (por exemplo, violino, saxofone, piano)
- Objetos domésticos (por exemplo, televisão, sofá, mesa, telefone)

### **Divisão de Dados**

- O conjunto de dados CIFAR-100 é dividido em conjuntos de treinamento e teste, com 50.000 imagens de treinamento e 10.000 imagens de teste. Cada imagem é representada como um tensor de três canais (RGB) com dimensões 32x32 pixels.

### **Objetivo**

- O objetivo do CIFAR-100 é fornecer um conjunto de dados desafiador para avaliar algoritmos de classificação de imagens em um cenário de classificação multiclasse com um grande número de classes.

### **Referência**

O conjunto de dados CIFAR-100 foi coletado e mantido pelo Laboratório de Aprendizado Automático da Universidade de Toronto (UTML). Mais informações sobre o conjunto de dados e suas aplicações podem ser encontradas em: [CIFAR-100.](https://www.cs.toronto.edu/~kriz/cifar.html)



# REDE NEURAL 
<div>
  <p align="center">
        <img src='https://github.com/ViniciusSilveiraCampos/Classificador-De-Imagens/assets/108243297/90f0787d-c903-4093-85b2-8bea84992dec' width="408.5px" height="408.5px"  >


A rede neural de classificação implementada neste projeto utiliza uma arquitetura convolucional para processar imagens coloridas de entrada e realizar a classificação em um conjunto de 10 categorias diferentes. Aqui está uma visão geral das camadas e operações incluídas na rede:

- Camadas Convolucionais: A rede começa com duas camadas convolucionais, cada uma seguida por uma função de ativação ReLU para introduzir não-linearidade. Essas camadas são responsáveis por extrair características das imagens de entrada.

- Camadas de Pooling: Após cada camada convolucional, uma camada de pooling máxima é aplicada para reduzir a dimensionalidade das características extraídas e fornecer invariância a pequenas mudanças de posição nos objetos das imagens.

- Normalização por Lotes: A normalização por lotes é aplicada após cada camada de convolução para acelerar o treinamento e melhorar a estabilidade da rede.

- Camadas Totalmente Conectadas: Após as camadas convolucionais e de pooling, as características são achatadas em um vetor unidimensional e passadas através de duas camadas totalmente conectadas. Essas camadas têm como objetivo aprender representações mais abstratas das características extraídas.

- Dropout: Dropout é aplicado antes das camadas totalmente conectadas para regularização e prevenir o overfitting, desligando aleatoriamente neurônios durante o treinamento.

- Camada de Saída: Finalmente, uma camada de saída linear é aplicada para gerar as previsões finais. A rede é treinada usando a função de perda de entropia cruzada e o otimizador Adam para atualizar os pesos durante o treinamento.
