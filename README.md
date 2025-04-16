
# Processamento de Imagens - Visão Computacional

## Como Executar

Para executar o processamento da imagen e gerar o relatório:

```
executar o codigo pelo colab, alterando a variavel nome_arquivo para a imagem que deseja carregar
```

## Etapas do Processamento

Carregamento da imagem original
A imagem é lida do arquivo para ser processada.

Conversão de BGR para RGB
O OpenCV carrega imagens no formato BGR, então convertê-la para RGB garante a visualização correta com matplotlib.

Aplicação de blur
Um desfoque leve (média 5x5) é aplicado para reduzir ruídos e suavizar a imagem.

Conversão para escala de cinza
Transforma a imagem colorida em tons de cinza, facilitando o processamento e análise.

Binarização
Um threshold é aplicado para separar objetos do fundo, criando uma imagem binária (preto e branco invertido).

Operações morfológicas:

Dilatação – Expande áreas brancas, preenchendo falhas e conectando regiões próximas.

Erosão – Contrai áreas brancas, eliminando pequenos ruídos.

Abertura – Erosão seguida de dilatação, remove pequenos ruídos mantendo a forma dos objetos.

Fechamento – Dilatação seguida de erosão, fecha pequenos buracos nas regiões brancas.

Detecção de bordas
O algoritmo Canny detecta as bordas da imagem a partir dos gradientes.

Identificação de contornos
Contornos são extraídos da imagem binária após o fechamento, identificando as formas presentes.

Desenho dos contornos
Os contornos detectados são desenhados sobre a imagem original com destaque em azul, criando o resultado final.

## Resultados

![Imagem Girafa](https://raw.githubusercontent.com/galera33/lab6/main/girafa3.png)


