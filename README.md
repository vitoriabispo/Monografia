
# 👩🏾‍💻 monografia 👩🏾‍💻

⁉️ Este repositórico contém a implementação de *DCGANs (Deep Convolutional Generative Adversarial Networks)*. O código foi desenvolvido durante as disciplinas Monografia I e II no trabalho intitulado **"Geração de Imagens Citológicas Sintéticas Através de Redes Generativas Adversárias"**. O objetivo deste trabalho é *gerar imagens sintéticas de estruturas celulares com o uso de redes generativas*.

⁉️ O projeto consiste na implementação de duas DCGANs semelhantes. O primeiro modelo é treinado para aprender a representar duas estruturas celulares básicas, enquanto o segundo modelo é treinado para gerar as imagens das classes de interesse.

---

## 💡etapas do treinamento
- 🔬**Treinamento da primeira DCGAN:** A primeira DCGAN foi treinada do zero utilizando os dados do banco de dados SIPaKMeD (https://www.cs.uoi.gr/~marina/sipakmed.html). O treinamento é realizado até a 250ª época para reduzir a quantidade de ruídos nas imagens geradas e os pesos da última época são salvos para serem utilizados na segunda DCGAN.
- 🔬**Treinamento da segunda DCGAN:** A segunda DCGAN é inicializada com os pesos do gerador da primeira DCGAN. Esta segunda rede é treinada utilizando os dados do CRIC Cervix (https://database.cric.com.br), a partir do ponto de partida estabelecido pela primeira rede.

---

## 🤔 utilização
- 🔬 Após o treinamento da segunda DCGAN, os pesos do gerador são salvos, possibilitando a **utilização independente do segundo modelo para gerar a quantidade de imagens citológicas sintéticas desejada**.

---

## 💻 estrutura do repositório
- 💾`dcgan_padrao.ipynb`: Notebook contendo o código da primeira DCGAN.
- 💾`dcgan_pre_treinada.ipynb`: Notebook contendo o código da segunda DCGAN, a DCGAN pré-treinada.
- 💾`gerador_dcgan.ipynb`: Notebook contendo o gerador de imagens implementado para gerar a quantidade de imagens desejada através dos pesos da segunda DCGAN.
---

## 📝 links úteis
- 🔗 O **texto da Monografia** está disponível no seguinte link: https://www.monografias.ufop.br/handle/35400000/6370
- 🔗 O seguinte **guia de implementação** foi utilizado: https://pytorch.org/tutorials/beginner/dcgan_faces_tutorial.html

## 📩 contato
- ✉️ Email: vitmariasb@yahoo.com
