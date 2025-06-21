# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href="https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Administração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# Classificação de Grãos de Trigo com Machine Learning 🌾

## Grupo
*Preencha com o nome do grupo*

## 👨‍🎓 Integrantes:
- <a href="#">João José Domingues Siva</a>
- <a href="#">Laís Kondo Claus</a>
- <a href="#">Murílo Santana</a>
- <a href="#">William Ferreira</a>


## 👩‍🏫 Professores:
### Tutor(a)
- <a href="#">Nome do Tutor</a>
### Coordenador(a)
- <a href="#">Nome do Coordenador</a>

---

## 📜 Descrição
Este trabalho tem como objetivo automatizar a classificação de três tipos de grãos de trigo — **Kama**, **Rosa** e **Canadian** — utilizando algoritmos de aprendizado de máquina. Atualmente, esse processo é feito manualmente em muitas cooperativas agrícolas, sendo demorado e sujeito a erros. A solução proposta visa aumentar a produtividade e reduzir falhas humanas.

Adotamos a metodologia **CRISP-DM** para guiar todas as etapas do projeto:
- **Entendimento dos Dados:**
  - Utilizamos o *Seeds Dataset* com 210 amostras e 7 características físicas dos grãos (área, perímetro, comprimento do sulco, etc.).
  - Não foram encontrados valores ausentes e os dados estavam bem distribuídos, sem problemas relevantes de outliers.
- **Preparação dos Dados:**
  - Realizamos a **padronização** das variáveis para ajustar a escala, importante para algoritmos como SVM e KNN.
  - Dividimos os dados em **treino (70%)** e **teste (30%)**.
- **Modelagem:**
  - Testamos três algoritmos de classificação:
    - KNN
    - SVM
    - Random Forest
  - O modelo **Random Forest** apresentou a melhor acurácia já nos testes iniciais (~92%).
  - Utilizamos **Grid Search** para ajuste de hiperparâmetros, mantendo o Random Forest como o melhor modelo.

## 📊 Resultados
- **Random Forest**: Melhor desempenho, preciso, estável e com pouca necessidade de ajuste fino.
- **SVM**: Resultados estáveis.
- **KNN**: Pequena queda de desempenho após ajuste de hiperparâmetros.

## 🏁 Conclusão
O modelo Random Forest se mostrou a melhor escolha para a tarefa de classificação dos grãos de trigo. Em um cenário real, essa solução pode ser integrada a sensores para agilizar o processo, aumentar a produtividade e reduzir erros humanos nas cooperativas agrícolas.

---

## 📁 Estrutura de Pastas

- <b>Data/</b>: Conjunto de dados utilizados no projeto.
- <b>Cap3_Implementando_Scikit_learn.ipynb</b>: Notebook principal com todo o desenvolvimento do projeto.
- <b>README.md</b>: Guia e explicação geral sobre o projeto (este arquivo).

## 🔧 Como executar o código

**Pré-requisitos:**
- Python 3.x
- Bibliotecas: scikit-learn, pandas, numpy, matplotlib, seaborn (instale via `pip install -r requirements.txt` se disponível)

**Passos para execução:**
1. Clone este repositório.
2. Instale as dependências necessárias.
3. Execute o notebook `Cap3_Implementando_Scikit_learn.ipynb` para reproduzir as análises e resultados.

## 🗃 Histórico de lançamentos

* 1.0.0 - 20/06/2025
    * Versão final do projeto

## 📋 Licença

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>

> Projeto desenvolvido para fins acadêmicos, seguindo boas práticas de ciência de dados e aprendizado de máquina.

