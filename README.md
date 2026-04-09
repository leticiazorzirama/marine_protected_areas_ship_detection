# Ship detection in Marine Protected Areas
Computer vision project for detecting fishing vessels in optical remote-sensing imagery from Brazilian marine protected areas. The main area of interest is the Grandes Unidades Oceânicas. This is a project of the Applied Marine Studies Laboratory, University of Vale do Itajaí (UNIVALI).  

[lema.acad.univali.br/site/](https://lema.acad.univali.br/site/)

---

## Estrutura de Diretórios

```
projeto_deteccao_barcos/
│
├── 1 documentos/
│   ├── 1.1 esqueleto_diretorios/ 
│   ├── 1.2 roadmap
│   ├── 1.3 relatorios/
│   └── 1.4 reunioes/
│
├── 2 revisao_literatura/
│   ├── 2.1 revisoes/
│   ├── 2.2 algoritmos/
│   └── 2.3 bases_publicas/
│
├── 3 dados_brutos/
│   ├── 3.1 grandes_unidades_oceanicas/
│   │   └── 3.1.1 limites_areas/
│   ├── 3.2 hotspots_pesca/
│   │   ├── 3.2.1 PREPS/
│   │   └── 3.2.2 GFW/
│   ├── 3.3 portos_marinhos_brasil/
│   │   ├── 3.3.1 MPA/
│   │   ├── 3.3.2 MMA/
│   │   ├── 3.3.3 GFW/
│   │   └── 3.3.4 LEMA/
│   └── 3.4 imagens_satelitais/
│       ├── 3.4.1 google_earth_engine/
│       ├── 3.4.2 google_earth_pro/
│       ├── 3.4.3 airbus/
│       └── 3.4.4 planet/
│
├── 4 processamentos/
│
├── 5 bases_de_dados/
│   ├── 5.1 base1_algoritmos/
│   ├── 5.2 base2_publica_deteccao_barcos/
│   ├── 5.3 base3_custom_deteccao_barcos_pesca_brasil/
│   └── 5.4 base4_portos_pesca_brasil/
│
├── 6 pipeline_modelos/
│   ├── 6.1 modelo_a/
│   │   ├── 6.1.1 src/
│   │   ├── 6.1.2 configs/
│   │   ├── 6.1.3 checkpoints/
│   │   └── 6.1.4 results/
│   └── 6.2 modelo_b/
│       ├── 6.2.1 src/
│       ├── 6.2.2 configs/
│       ├── 6.2.3 checkpoints/
│       └── 6.2.4 results/
│
├── 7 pipeline_avaliacao/
│   ├── 7.1 pipeline/
│   ├── 7.2 metricas/
│   ├── 7.3 comparativo_modelos/
│   └── 7.4 visualizacoes/
│
├── 8 produto_final/
│   ├── 8.1 pipeline/
│   ├── 8.2 api_ou_interface/
│   └── 8.3 documentacao_ao_usuario_final/
│
└── 9 outros/
```

---

## Descrição dos Diretórios

### 1 documentos/
Armazena a documentação geral do projeto.
- **1.1 esqueleto_diretorios/** — Estrutura de diretórios do projeto
- **1.1 roadmap** — Planejamento e cronograma do projeto
- **1.2 relatorios/** — Produções escritas relatando a execução do projeto para fins de relatórios e dissertações a serem entregues às partes interessadas (LEMA, BNA, MCA, FAPESC) 
- **1.3 reunioes/** — Atas e registros de reuniões

### 2 revisao_literatura/
Levantamentos sistemáticos da literatura científica acerca do problema de pesquisa: detecção de embarcações com algoritmos de aprendizado profundo a partir de imagens ópticas de satélite.
- **2.1 revisoes/** — Revisões existentes
- **2.2 algoritmos/** — Levantamento de algoritmos consolidados (levantamento consolidará a Base 1 encontrada em bases_de_dados/base1_algoritmos/)
- **2.3 bases_publicas/** — Levantamento de bases de dados públicas (levantamento consolidará a Base 2 encontrada em bases_de_dados/base2_publica_deteccao_barcos/)

### 3 dados_brutos/
Fontes primárias de dados brutos compilados, minimamente processados. **Estes arquivos nunca devem ser modificados.**
- **3.1 grandes_unidades_oceanicas/** — Dados de limites das áreas de interesse do projeto
- **3.2 hotspots_pesca/** — Dados de hotspots de pesca (PREPS, GFW)
- **3.3 portos_marinhos_brasil/** — Dados de portos pesqueiros marinhos do Brasil (MPA, MMA, GFW, LEMA)
- **3.4 imagens_satelitais/** — Imagens satelitais de múltiplas fontes (Google Earth Engine, Google Earth Pro, Airbus, Planet)

### 4 processamentos/ 
Etapas intermediárias de transformação e preparação dos dados brutos. A ser estruturado conforme o projeto avança.

### 5 bases_de_dados/
Bases de dados customizadas e consolidadas.
- **5.1 base1_algoritmos/** — Base de algoritmos construída no levantamento sistemático (encontra-seem revisao_literatura/algoritmos/)
- **5.2 base2_publica_deteccao_barcos/** — Base pública de detecção de barcos (encontra-se em revisao_literatura/bases_publicas/)
- **5.3 base3_custom_deteccao_barcos_pesca_brasil/** — Base customizada de detecção de barcos da pesca brasileira em áreas marinhas
- **5.4 base4_portos_pesca_brasil/** — Base de portos pesqueiros do Brasil

### 6 pipeline_modelos/
Implementação dos modelos de detecção.
- **src/** — Código-fonte do modelo
- **configs/** — Hiperparâmetros e arquivos de configuração
- **checkpoints/** — Pesos e estados salvos durante o treinamento
- **results/** — Resultados e saídas geradas pelo modelo

### 7 pipeline_avaliacao/
Avaliação e comparação centralizada dos modelos.
- **7.1 pipeline/** — Pipeline de avaliação
- **7.2 metricas/** — Métricas de desempenho
- **7.3 comparativo_modelos/** — Análise comparativa entre os modelos
- **7.4 visualizacoes/** — Gráficos e visualizações dos resultados

### 8 produto_final/
Entregável final do projeto.
- **8.1 pipeline/** — Pipeline unificado de inferência
- **8.2 api_ou_interface/** — API ou interface de uso
- **8.3 documentacao_ao_usuario_final/** — Documentação para o usuário final

### 9 scripts/
Scripts de apoio, automação e prototipagem utilizados ao longo do projeto.

---

## Observações
**Publicidade e limite de armazenamento**
Arquivos privados ou que ultrapassam o limite de armazenamento no repositório do Github estarão incluídos no .gitignore.
