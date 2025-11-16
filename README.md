# Projeto Integrado de Classificação Supervisionada — UMC

**Disciplina:** Inteligência Artificial — Prof. Dr. Fabiano Menegidio  
**Projeto:** IA para salvar vidas: avaliação comparativa de modelos de classificação supervisionada  
**Autores:** ALYSON RODRIGO MIGUEL PEREIRA  
**Instituição:** Centro Universitário UMC

## Resumo
Este repositório contém o código e material complementar do projeto que compara modelos de classificação supervisionada aplicados aos datasets Titanic (pedagógico) e Breast Cancer Wisconsin (diagnóstico). Foram avaliados XGBoost, SVM (RBF), Random Forest e HistGradientBoostingClassifier, com pré-processamento, busca de hiperparâmetros e análise de interpretabilidade.

## Estrutura do repositório
- `notebook_projeto_integrado.ipynb` — Notebook principal (Google Colab), com todos os experimentos e plots.  
- `README.md` — Este arquivo.  
- `img/` — Gráficos e imagens geradas (ROC, PR, matrizes de confusão, importâncias).  
- `doc/` — Documentos finais: `resumo_expandido_projeto_IA.docx` / `resumo_expandido_projeto_IA.pdf` e `poster.pdf`.  
- `models/` — Modelos treinados (.joblib).  

## Como reproduzir (Google Colab)
1. Abra o `notebook_projeto_integrado.ipynb` no Google Colab.  
2. Em *Runtime → Change runtime type*, mantenha Python 3 (GPU não é necessária).  
3. Execute as células na ordem. Observação: as buscas por hiperparâmetros foram reduzidas para tornar a execução prática; aumente `n_iter`/grades se quiser melhores resultados.  
4. As figuras geradas são salvas automaticamente em `img/` e os modelos salvos em `models/`.

## Dependências
Recomenda-se Python >=3.8. Principais bibliotecas:
- scikit-learn
- xgboost
- shap
- seaborn
- pandas
- matplotlib
- joblib

Instale com:
```bash
pip install scikit-learn xgboost shap seaborn pandas matplotlib joblib
