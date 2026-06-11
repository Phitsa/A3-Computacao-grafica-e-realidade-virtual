# Detecção de Semáforos com OpenCV

Este projeto foi desenvolvido em **Python**, utilizando **OpenCV**, **NumPy** e **Matplotlib**, com o objetivo de demonstrar técnicas de **Visão Computacional** aplicadas à detecção de semáforos por meio do processamento de imagens.

O algoritmo realiza o pré-processamento da imagem, segmentação por cores, detecção de contornos e análise de circularidade para identificar as luzes do semáforo.

---

# 🚀 Funcionalidades

O projeto executa as seguintes etapas:

* Leitura da imagem de entrada;
* Redimensionamento para 640×480 pixels;
* Normalização dos valores dos pixels para melhorar o contraste;
* Conversão para escala de cinza;
* Segmentação das cores vermelha, amarela e verde utilizando o espaço de cores HSV;
* Detecção de contornos nas regiões segmentadas;
* Verificação da circularidade dos objetos encontrados;
* Detecção de bordas utilizando o algoritmo de Canny;
* Exibição das etapas intermediárias e do resultado final.

---

# 🛠️ Requisitos

* Python 3.7 ou superior

Bibliotecas necessárias:

```bash
pip install opencv-python numpy matplotlib
```

---

# ▶️ Executando no Google Colab

1. Abra o notebook no Google Colab;
2. Faça o upload da imagem que será utilizada;
3. Ajuste o caminho da imagem, se necessário;
4. Execute todas as células do notebook.

---

# ▶️ Executando Localmente

Caso utilize Jupyter Notebook ou VS Code:

1. Instale as dependências:

```bash
pip install opencv-python numpy matplotlib jupyter
```

2. Abra o notebook normalmente.

3. Caso esteja utilizando `cv2_imshow`, substitua por:

```python
cv2.imshow("Imagem", img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

ou utilize:

```python
plt.imshow(cv2.cvtColor(img, cv2.COLOR_BGR2RGB))
plt.show()
```

para exibir as imagens.

---

# 📚 Tecnologias Utilizadas

* Python
* OpenCV
* NumPy
* Matplotlib
* Jupyter Notebook / Google Colab

---

# 🎯 Objetivo

Demonstrar técnicas básicas de Visão Computacional para reconhecimento de características visuais de um semáforo, utilizando operações de pré-processamento, segmentação por cores, detecção de contornos e análise geométrica.
