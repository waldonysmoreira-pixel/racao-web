# racao-web
# Formulador de Ração 1.0 — Web (Streamlit)

Este app lê sua planilha “NOVO MODELO DE TABELAS.xlsx”, calcula exigências (calibradas pela aba EXIGENCIAS), sugere dieta, mostra aportes, custos e déficits, e permite exportar relatório. Também inclui o histórico da aba DIETAS.

## Como rodar no Streamlit Cloud
1. Suba este repositório ao GitHub.
2. Acesse https://streamlit.io/cloud e crie um app novo selecionando este repo.
3. Deixe o path do arquivo principal como `app_web.py`.
4. Ao iniciar, o app estará online sem instalar nada localmente.

## Pastas e arquivos
- `data/NOVO MODELO DE TABELAS.xlsx`: sua planilha original (necessária).
- `racao/`: módulos de dados e cálculo.
- `app_web.py`: ponto de entrada do app.

## Observações
- A leitura da aba EXIGENCIAS faz parsing e interpolação simplificados; se o layout variar muito, ajuste `racao/exigencias.py`.
- Para usar outro arquivo de planilha, substitua o arquivo em `data/`.
