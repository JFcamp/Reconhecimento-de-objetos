# Detecção de Objetos com YOLOv8

Este projeto demonstra como utilizar o modelo YOLOv8 para realizar a detecção de objetos em tempo real através de uma webcam. O código usa a biblioteca `ultralytics` para carregar o modelo e fazer previsões.

## Requisitos

Antes de executar o código, você precisa instalar as dependências necessárias. Certifique-se de ter o Python instalado e execute o seguinte comando para instalar a biblioteca `ultralytics`:

```bash
pip install ultralytics
```
## Codigo
Aqui está o código completo para realizar a detecção de objetos com o YOLOv8:


```bash
from ultralytics import YOLO

# Carregar o modelo YOLOv8
modelo = YOLO('yolov8n.pt')

# Realizar predições utilizando a webcam (source='0') e mostrar os resultados na tela
modelo.predict(source='0', show=True)
```
## Explicação do codigo
1-Importação da Biblioteca: Importa a biblioteca ultralytics que contém a implementação do YOLOv8.

```bash
from ultralytics import YOLO
```

2-Carregamento do Modelo: Importa a biblioteca ultralytics que contém a implementação do YOLOv8.


```bash
modelo = YOLO('yolov8n.pt')
```
3- Realização de Predições: Utiliza a webcam (especificada por source='0') para capturar imagens em tempo real e realizar a detecção de objetos. O parâmetro show=True exibe as imagens com as detecções sobrepostas na tela.

```bash
modelo.predict(source='0', show=True)
```

## Observações
-Certifique-se de que a sua webcam está funcionando corretamente.
-Para usar um vídeo pré-gravado ou imagens estáticas em vez de uma webcam, substitua '0' pelo caminho do arquivo de vídeo ou da imagem.
-Para melhores resultados, você pode explorar outros modelos YOLOv8 disponíveis ou ajustar os parâmetros de predição conforme necessário.
