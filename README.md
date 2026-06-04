# 🌱 SP Verde & Ar — Monitoramento da Qualidade do Ar e Arborização Urbana em São Paulo

> **Projeto Extensionista com Dados** — AE1 | Projeto Integrador  
> Disciplina: Projeto Integrador — 2026

---

## 📋 Sobre o Projeto

Este projeto analisa a **distribuição espacial da arborização urbana** e da **qualidade do ar** nos 96 distritos do município de São Paulo (SP), identificando correlações, desigualdades territoriais e oportunidades de intervenção socioambiental.

O trabalho tem caráter **extensionista**: os produtos gerados (dashboard, dataset aberto e relatório técnico) serão disponibilizados gratuitamente para moradores, ONGs e gestores públicos.

---

## 🎯 Objetivos

- Coletar e consolidar dados públicos de arborização (GeoSampa/PMSP) e qualidade do ar (CETESB)
- Construir indicadores de **déficit de arborização** e **exposição à poluição** por faixa de renda/IDH distrital
- Identificar os **10 distritos com maior vulnerabilidade socioambiental**
- Publicar os dados tratados em formato aberto (CSV + GeoJSON)

---

## ❓ Perguntas Analíticas

| # | Pergunta |
|---|----------|
| PA1 | Quais distritos apresentam simultaneamente menor cobertura arbórea e piores índices de qualidade do ar? |
| PA2 | Existe correlação significativa entre IDH distrital e cobertura de arborização pública? |
| PA3 | Como a concentração de PM2,5 varia sazonalmente nas regiões com menor arborização? |
| PA4 | Qual a proporção de população exposta a PM2,5 acima do limite da OMS por faixa de renda? |

---

## 📊 KPIs Principais

| KPI | Descrição |
|-----|-----------|
| **ICA** — Índice de Cobertura Arbórea | % de área distrital coberta por vegetação |
| **IEP** — Índice de Exposição à Poluição | Média anual de PM2,5 ponderada pela população do distrito |
| **IVSA** — Índice de Vulnerabilidade Socioambiental | Score 0–10 combinando ICA inverso + IEP + IDH inverso |

---


## 🗃️ Fontes de Dados

| Fonte | Dados | Link |
|-------|-------|------|
| **GeoSampa (PMSP)** | Cobertura vegetal e arborização por distrito | [geosampa.prefeitura.sp.gov.br](https://geosampa.prefeitura.sp.gov.br) |
| **CETESB** | Qualidade do ar: PM2,5, PM10, O3 (rede de estações) | [cetesb.sp.gov.br/ar](https://cetesb.sp.gov.br/ar) |
| **IBGE — Censo 2022** | Pop., renda per capita, IDH por setor censitário | [ibge.gov.br / SIDRA](https://sidra.ibge.gov.br) |
| **InfoSiga SP** | Dados de saúde (doenças respiratórias) | [infosiga.sp.gov.br](http://www.infosiga.sp.gov.br) |

Todos os dados utilizados são **públicos e de acesso livre**.

---

## 🚀 Como Executar

### Pré-requisitos

```bash
Python >= 3.10
pip install -r requirements.txt
```

### Instalar dependências

```bash
pip install pandas geopandas plotly dash folium scipy requests
```

### Rodar os notebooks

```bash
jupyter notebook notebooks/
```

### Rodar o dashboard

```bash
cd dashboard
python app.py
# Acesse: http://localhost:8050
```

---

## 📅 Cronograma

| Semana | Fase | Entregável |
|--------|------|------------|
| S1–S2 | Iniciação | Termo de Abertura (AE1) ✅ |
| S3–S4 | Coleta | Datasets brutos organizados |
| S5–S6 | Preparação | Dataset integrado e limpo |
| S7–S8 | Análise | Notebooks analíticos |
| S9–S10 | Visualização | Dashboard + relatório PDF |
| S11–S12 | Comunicação e encerramento | Entrega final + publicação |

---

## 🔒 Aspectos Éticos e LGPD

- ✅ Apenas **dados públicos e agregados** — nenhum dado pessoal individual é coletado
- ✅ Dados de saúde utilizados apenas em nível **distrital agregado**
- ✅ Base legal LGPD: **Art. 7º, II** — dados tornados públicos pelo poder público
- ✅ Todos os scripts publicados com **licença aberta (MIT)**
- ✅ Resultados divulgados em formatos acessíveis para comunidades vulneráveis

---

## 📁 Documentação do Projeto

- 📄 [Termo de Abertura + Briefing (AE1)](./docs/escopo-1/AE1/AE1_Projeto_Extensionista.pdf)

---

## 👥 Equipe

| Nome | Papel |
|------|-------|
| Jekson Cuna | Analista de Dados |

---

## 📜 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).  
Os dados produzidos são disponibilizados sob [Creative Commons CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

---

## 🤝 Contribuições

Contribuições são bem-vindas! Abra uma *issue* ou envie um *pull request*.

---

*Projeto desenvolvido como atividade extensionista — Disciplina Projeto Integrador com Dados, 2026.*
