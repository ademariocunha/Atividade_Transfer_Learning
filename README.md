# Transfer Learning com TensorFlow: Classificador de Gatos e Cachorros

Este repositório apresenta um projeto simples de Transfer Learning utilizando TensorFlow para classificar imagens de gatos e cachorros. O modelo foi treinado com o dataset [Cats and Dogs Filtered](https://storage.googleapis.com/mledu-datasets/cats_and_dogs_filtered.zip).


## Requisitos
Certifique-se de ter o Python 3.8 ou superior instalado. As dependências do projeto incluem:

- TensorFlow
- matplotlib
- Pillow
- requests
- numpy

3. **Classificar uma Imagem via URL:**
   Substitua o link da imagem no final do script pelo URL desejado e execute novamente o script. Exemplo:
   ```python
   image_url = "https://upload.wikimedia.org/wikipedia/commons/3/3a/Cat03.jpg"
   classify_image(image_url, model)
   ```

## Funcionamento

1. **Treinamento:**
   O modelo base MobileNetV2 é utilizado para extrair features, seguido por uma camada de pooling global e uma densa para classificação binária (gato ou cachorro).

2. **Classificação de Imagem:**
   A imagem é baixada de uma URL, redimensionada para 160x160 pixels, normalizada e passada pelo modelo para prever se é um gato ou cachorro.

## Resultados
Durante o treinamento, a acurácia e a perda são exibidas. Após o treinamento, o modelo pode ser usado para classificar imagens individuais fornecendo um link para a imagem.

## Exemplos

### Predição de uma Imagem
#### Entrada:
URL: [Cat Image](https://upload.wikimedia.org/wikipedia/commons/3/3a/Cat03.jpg)

#### Saída:
- Predição: **Gato**
- Confiança: **99%**

![Resultado](https://upload.wikimedia.org/wikipedia/commons/3/3a/Cat03.jpg)

## Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.

## Licença
Este projeto está licenciado sob a [MIT License](LICENSE).

