
# 🧠 Redes Neurais - MLP FeedForward com Perceptron

Este projeto implementa um **Perceptron Simples** para classificação binária utilizando o modelo **MLP Feedforward** com base em um dataset externo. A rede é treinada com um conjunto de dados (80%) e testada com o restante (20%), retornando a acurácia final.

---

## 📁 Estrutura do Projeto

- `redes_neurais_mlp_feedforward.py` — Código principal com toda a lógica do Perceptron.
- `data.csv` — Arquivo necessário contendo os dados para treino e teste. (Você precisa fornecê-lo no mesmo diretório).

---

## ⚙️ Como funciona?

1. **Carregamento do dataset** (`data.csv`) contendo valores numéricos.
2. **Separação dos dados** em treino e teste (função `treino_teste_split`).
3. **Treinamento do Perceptron** com `perceptron_fit`.
4. **Validação do modelo** com `perceptron_predict`.
5. **Cálculo da acurácia** com `acuracia`.

---

## ▶️ Executando localmente

### Pré-requisitos

- Python 3.7+
- Arquivo `data.csv` no mesmo diretório contendo os dados de entrada, com a seguinte estrutura:
  ```
  classe,x1,x2
  -1,0.1,0.5
  1,0.9,0.8
  ...
  ```

### Como executar

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
python redes_neurais_mlp_feedforward.py
```

---

## 📊 Executando no Google Colab

1. Acesse o notebook original no Colab:  
   [Abrir no Google Colab](https://colab.research.google.com/drive/10eiFcNGhhwusbVbBhzemvtUqrbarLoiQ)
2. Faça upload do arquivo `data.csv` via botão lateral do Colab.
3. Execute as células sequencialmente.

---

## 📌 Observações

- O algoritmo é sensível à qualidade do dataset. Certifique-se de que os dados estejam normalizados e corretamente rotulados.
- A taxa de aprendizado é fixa em `0.01`, e o número máximo de épocas é `1000`.

---

## 📈 Exemplo de saída

```python
[0.47, 0.62, 0.15] # Pesos iniciais
512 # Número de épocas até a convergência
[1, -1, 1, -1, ...] # Previsões
0.85 # Acurácia final
```

---

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se livre para abrir issues ou pull requests com melhorias, novos datasets ou ajustes na lógica da rede.

---

## 📜 Licença

Este projeto está licenciado sob a licença MIT.
