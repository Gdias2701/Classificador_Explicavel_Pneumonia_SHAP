🩺 Classificador de Pneumonia Explicável com SHAP

Este repositório contém um modelo de classificação de pneumonia em imagens de raios-X de tórax, desenvolvido com redes neurais convolucionais (CNNs). Além da predição, o projeto utiliza a biblioteca SHAP (SHapley Additive exPlanations) para fornecer explicabilidade aos resultados, indicando quais regiões da imagem tiveram maior influência na decisão do modelo.

🧩 Objetivo

Construir um classificador robusto para detecção de pneumonia.

Tornar o modelo explicável, facilitando a interpretação médica.

Demonstrar como ferramentas de interpretabilidade podem ser integradas a modelos de deep learning em imagens médicas.

⚙️ Tecnologias Utilizadas

Python 

TensorFlow / Keras – para construção e treinamento da CNN

OpenCV / PIL – para manipulação das imagens

Matplotlib / Seaborn – para visualização

SHAP – para explicabilidade das predições

🎯 Funcionamento do Modelo

Pré-processamento das imagens: normalização, redimensionamento e separação em treino/validação/teste.

Treinamento da CNN: arquitetura multicamada com softmax na saída para classificação binária (pneumonia vs normal).

Explicabilidade com SHAP:

Cálculo dos valores de importância de cada pixel/região.

Geração de mapas de calor sobre as imagens indicando as áreas mais relevantes para a predição.

Exemplo de saída explicável:

Imagem original (raio-X de tórax)

Mapa de ativação SHAP destacando regiões pulmonares que influenciaram a decisão
