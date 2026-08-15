# Auditoria de Produto nº 01 — Kit NR-1 Riscos Psicossociais

**Data:** 14/08/2026
**Produto:** KIT_NR1_RISCOS_PSICOSSOCIAIS — 37 arquivos (14 POPs, 7 formulários, 10 ferramentas, 6 bônus)
**Norma de referência:** NR-1 consolidada (texto atualizado 2025), com as redações das Portarias MTE nº 1.419, de 27/08/2024, e nº 765, de 15/05/2025
**Status:** auditoria **executada** sobre os arquivos reais

> **Veredito:** o kit está **atualizado quanto ao prazo e à base legal** — bem acima da média do mercado. As não conformidades encontradas **não são de desatualização**; são de **enquadramento normativo** e de **controle de documentos**. Duas delas comprometem a rastreabilidade que é justamente a promessa central do produto.

---

## 1. Método

Extração integral do texto dos 37 arquivos (docx/xlsx/pptx) e varredura cruzada contra o texto consolidado da NR-1. Foram verificados: base legal citada, datas de vigência, numeração de itens da norma, campos obrigatórios do inventário, critérios de avaliação de risco, prazos de retenção, integridade de referências cruzadas entre documentos, tratamento de dados pessoais sensíveis e delimitação de escopo clínico.

---

## 2. Correção da base normativa — o que o texto consolidado mostrou

Registro aqui as correções em relação ao que eu havia escrito na versão anterior deste documento, porque elas mudam o conteúdo técnico da correção:

| Ponto | Correção |
|---|---|
| **Data de vigência** | O correto é **26/05/2026** — que é o que o kit usa, de forma consistente, em 19 ocorrências. Meu "25/05/2026" vinha de fonte secundária que descrevia o fim do prazo anterior, não o início da vigência. O kit está certo. |
| **Data da Portaria 765** | É de **15/05/2025** (publicada no DOU em 16/05/2025). |
| **Itens numerados** | Agora confirmados no texto consolidado — deixam de ser incerteza e viram instrumento de auditoria. |

**Os três itens que sustentam a exigência de FRPRT:**

- **1.5.3.1.4** — "O gerenciamento de riscos ocupacionais deve abranger os riscos que decorrem dos agentes físicos, químicos, biológicos, riscos de acidentes e riscos relacionados aos **fatores ergonômicos, incluindo os fatores de risco psicossociais relacionados ao trabalho**."
- **1.5.3.2.1** — "A organização deve considerar as condições de trabalho, nos termos da **NR-17**, incluindo os fatores de risco psicossociais relacionados ao trabalho."
- **1.5.4.4.5.3** — "Para a probabilidade de ocorrência das lesões ou agravos à saúde decorrentes de **fatores ergonômicos, incluindo os fatores de riscos psicossociais** relacionados ao trabalho, a avaliação de risco deve considerar **as exigências da atividade de trabalho e a eficácia das medidas de prevenção implementadas**."

**A leitura que muda o produto:** a NR-1 **não** criou uma categoria autônoma de risco psicossocial. Ela alojou os FRPRT **dentro dos fatores ergonômicos**. Isso não é detalhe de redação — determina onde o risco entra no inventário e, principalmente, **qual critério de probabilidade é válido**.

**E os dois itens de documentação:**

- **1.5.7.3.2** — o inventário deve contemplar, no mínimo, nove informações (alíneas "a" a "i").
- **1.5.7.3.3.1** — "O histórico das atualizações deve ser mantido por um período mínimo de **20 (vinte) anos**."

---

## 3. O que o kit já faz certo

Auditoria não é só lista de defeito. Estes pontos estão conformes e vários são diferenciais reais:

| Verificação | Resultado |
|---|---|
| Portaria 1.419/2024 citada | ✔ 60 ocorrências, em 25 dos 37 arquivos |
| Data de vigência correta e consistente | ✔ 26/05/2026 em 19 ocorrências, **zero** ocorrências de data antiga |
| Nenhum resíduo de "fase educativa em curso" | ✔ todas as menções estão no passado, corretamente |
| LGPD | ✔ art. 5º, II e art. 11 citados, DPO, dado sensível, acesso restrito, trilha de auditoria |
| Anonimato do questionário | ✔ vedação de matrícula, e-mail, IP e geolocalização; urna coletiva na versão física |
| Delimitação de escopo clínico | ✔ avaliação clínica é competência exclusiva do médico do trabalho (POP-013) |
| Interface com PCMSO / NR-7 | ✔ presente e bem construída no POP-013 |
| Lei nº 14.457/2022 (CIPA / assédio) | ✔ 48 ocorrências |
| ISO 45003 como referência técnica | ✔ 25 ocorrências |
| Integridade das referências entre POPs | ✔ os 14 POPs e 7 formulários citados existem — zero referência órfã |
| Estrutura de 15 seções com RACI, KPIs, histórico de revisões | ✔ em todos os 14 POPs |
| Sem identidade visual da Leval | ✔ zero ocorrências |

Nenhuma das lacunas que eu havia levantado como hipótese na versão anterior se confirmou. O kit não estava desatualizado.

---

## 4. Não conformidades

### 🔴 NC-01 — Colisão de códigos de formulário entre os POPs e os formulários entregues
**Gravidade: crítica. É o achado principal.**

Os códigos `FOR-PSI-001` a `FOR-PSI-007` são usados na seção 12 de cada POP como numeração **local**, reiniciando a cada procedimento — mas a pasta `/Formularios` entrega sete documentos com **esses mesmos códigos** e significados fixos. O mesmo código aponta para documentos diferentes conforme o POP que se está lendo.

| Código | Formulário entregue | POP-PSI-001 usa como | POP-PSI-003 usa como |
|---|---|---|---|
| FOR-PSI-001 | Relato de Ocorrência Psicossocial | Lista de Levantamento de Perigos | Ata de aprovação da Alta Direção |
| FOR-PSI-003 | Ata de Análise Crítica da Direção | Planilha de indicadores (CID-F, turnover) | — |
| FOR-PSI-004 | Termo de Compromisso da Alta Direção | Registro de observação direta | Inventário e Matriz de Classificação |
| FOR-PSI-005 | Registro de Atendimento de Acolhimento | Ata de validação SESMT/CIPA | Inventário geral do GRO/PGR |

Agrava: o POP-PSI-006 usa `FOR-PSI-005` para **três registros diferentes** na mesma tabela. E o problema é irregular — o POP-006 acerta os códigos 001 e 002, o que faz o esquema parecer correto até alguém cruzar.

**Por que é crítico:** rastreabilidade documental é a promessa do produto. Um auditor-fiscal ou auditor de certificação que seguir a referência encontra documento trocado. E é o tipo de defeito que o cliente descobre depois de implantar.

**Correção:** separar os espaços de codificação. Formulários entregues mantêm `FOR-PSI-0XX`. Os registros internos de cada POP passam a `REG-PSI-<nºPOP>-<seq>` — ex.: `REG-PSI-001-01`. Onde o registro **é** um formulário entregue, citar o código global. Correção mecânica, alto impacto.

---

### 🟠 NC-02 — Retenção de 5 anos onde a norma exige 20
**Item 1.5.7.3.3.1**

O POP-PSI-003 define **5 anos** para o "Inventário e Matriz de Classificação de Riscos Psicossociais (critérios, classificação por setor/função e priorização)". Esse registro **é** dado de inventário — a alínea "i" (avaliação e classificação) e a alínea "f" do 1.5.7.3.2. A NR-1 exige que o histórico das atualizações do inventário seja mantido por **no mínimo 20 anos**.

O kit acerta ao marcar "Permanente" para o inventário geral integrado, mas a matriz de classificação — que é onde mora o critério e o histórico — fica em 5 anos.

**Correção:** 20 anos (ou "Permanente") para todo registro que componha o inventário ou seu histórico de atualização. Revisar a tabela de retenção dos 15 documentos: hoje há 54 ocorrências de "5 anos", 12 "Permanente", 5 "10 anos", 2 "3 anos" e apenas 2 "20 anos", sem critério declarado.

---

### 🟠 NC-03 — FRPRT tratado como categoria autônoma, não como fator ergonômico
**Itens 1.5.3.1.4 e 1.5.4.4.5.3**

A expressão "fator ergonômico" não aparece **nenhuma vez** nos 37 arquivos. O kit trata FRPRT como uma família de risco independente, com inventário próprio e paralelo ("INVENTÁRIO DE RISCOS PSICOSSOCIAIS — ESTRUTURA DO PGR").

A norma faz o oposto: coloca os FRPRT **dentro** dos fatores ergonômicos, no mesmo inventário único do PGR.

**Consequência prática:** um PGR com dois inventários paralelos é vulnerável em fiscalização — o auditor pede o inventário de riscos ocupacionais, singular, do 1.5.7.3.1.

**Correção:** reposicionar como bloco de **fatores ergonômicos — FRPRT** dentro do inventário único, mantendo a planilha atual como ferramenta de trabalho. O Anexo III do POP-003 (correspondência entre matrizes) já é o embrião disso — falta o enquadramento explícito.

---

### 🟠 NC-04 — Critério de probabilidade não segue o que a norma determina
**Item 1.5.4.4.5.3**

A planilha usa escala genérica ("4 - Provável", "3 - Possível") — a mesma lógica de risco de acidente. Mas a NR-1 é específica: para fatores ergonômicos e FRPRT, a probabilidade deve considerar **as exigências da atividade de trabalho** e **a eficácia das medidas de prevenção implementadas**.

O POP-003 chega perto: manda "estabelecer critérios próprios, distintos da matriz tradicionalmente usada para riscos físicos". Está certo na intenção, mas não ancora no critério da norma — e a planilha entregue não implementa nenhum dos dois.

**Correção:** substituir a escala de probabilidade por uma ancorada nos dois vetores do 1.5.4.4.5.3, com a coluna "Medidas Existentes" (que já existe) alimentando o vetor de eficácia. Este é o item que mais eleva o nível técnico do kit — quase nenhum concorrente faz.

---

### 🟠 NC-05 — Inventário sem quatro dos nove campos obrigatórios
**Item 1.5.7.3.2**

| Alínea | Exigência | Planilha |
|---|---|---|
| a | caracterização dos processos e ambientes de trabalho | **ausente** |
| b | caracterização das atividades | **ausente** |
| c | descrição dos perigos, com fontes e/ou circunstâncias | ✔ |
| d | possíveis lesões ou agravos | ✔ parcial |
| e | grupos de trabalhadores expostos | ✔ |
| f | medidas de prevenção implementadas | ✔ |
| g | caracterização da exposição dos trabalhadores | **ausente** |
| h | resultados da avaliação de ergonomia nos termos da NR-17 | **ausente** |
| i | avaliação dos riscos, incluindo classificação | ✔ |

**Correção:** quatro colunas novas. A alínea "h" é a mais relevante e leva à NC-06.

---

### 🟡 NC-06 — Sem vínculo operacional com a avaliação ergonômica da NR-17

"AET" aparece **uma vez** em todo o kit, apenas como verbete de glossário no POP-001. "AEP" não aparece. Como a alínea "h" do 1.5.7.3.2 exige os resultados da avaliação de ergonomia no inventário, e o 1.5.3.2.1 remete expressamente à NR-17, falta a ponte que conecta o levantamento de FRPRT à avaliação ergonômica que a empresa já é obrigada a ter.

**Correção:** seção no POP-001 definindo como o levantamento de FRPRT consome e alimenta a AEP/AET, e coluna de referência cruzada no inventário.

---

### 🟡 NC-07 — Anonimato sem piso de agregação

O kit garante anonimato de forma consistente e determina resultados agregados "por setor ou equipe". Não define **número mínimo de respondentes por recorte**. Sem esse piso, um setor de três pessoas divulgado separadamente é identificável — e o dado é sensível.

**Correção:** regra explícita — não divulgar recorte com menos de 5 respondentes; agregar ao nível superior quando não atingir o piso. Uma linha no POP-002 e uma trava na planilha de tabulação.

---

### 🟡 NC-08 — Base legal do tratamento ancorada em consentimento

O POP-002 manda "obter o consentimento informado do trabalhador". Em relação de emprego, consentimento é base legal frágil: há subordinação, e ele é revogável a qualquer tempo (art. 8º, §5º da LGPD). Se o trabalhador revoga, a empresa perde a base para tratar um dado que a NR-1 **obriga** a tratar.

**Correção:** declarar a base legal como **art. 11, II, "a"** — cumprimento de obrigação legal/regulatória pelo controlador, que é exatamente o caso da NR-1 — e reposicionar o consentimento informado como **transparência e ciência** (art. 9º), que é o papel legítimo dele aqui. O texto do POP-002 já manda informar "a base legal de tratamento"; basta dizer qual é.

---

### 🟡 NC-09 — CID extraído pelo RH sem salvaguarda de sigilo médico

O POP-001 instrui "extrair, junto ao RH e ao eSocial, os afastamentos por transtornos mentais (CID-10 grupo F)". O uso é epidemiológico e agregado — correto na finalidade. Mas o CID é protegido por sigilo médico, e a expressão "sigilo médico" não aparece em nenhum dos 37 arquivos.

**Correção:** rotear o dado nominal pelo médico do trabalho / PCMSO, que entrega ao PGR já agregado por setor, função e turno. Duas linhas no POP-001 — e fecha uma exposição real do cliente.

---

### 🟢 NC-10 — Portaria 765/2025 nunca citada

O kit afirma corretamente o fim da fase educativa em 26/05/2026, mas em nenhum arquivo cita a portaria que a estabeleceu. Quem perguntar "onde está escrito?" não encontra no material.

**Correção:** incluir "Portaria MTE nº 765, de 15/05/2025" nas referências normativas dos POPs e do Guia.

---

## 5. Plano de correção

| Ordem | Ação | Arquivos | Esforço |
|---|---|---|---|
| 1 | Recodificar registros internos (`REG-PSI-…`) — NC-01 | 14 POPs | Médio, mecânico |
| 2 | Corrigir retenções para 20 anos / Permanente — NC-02 | 15 docs | Baixo |
| 3 | Enquadrar FRPRT como fator ergonômico — NC-03 | POP-001, 003, planilha, Guia, PGR | Médio |
| 4 | Nova escala de probabilidade conforme 1.5.4.4.5.3 — NC-04 | POP-003 + planilha | Médio |
| 5 | Quatro colunas do 1.5.7.3.2 — NC-05 | Planilha inventário | Baixo |
| 6 | Ponte com AEP/AET — NC-06 | POP-001, planilha | Médio |
| 7 | Piso de agregação (n≥5) — NC-07 | POP-002 + planilha | Baixo |
| 8 | Base legal art. 11, II, "a" — NC-08 | POP-002, 006 | Baixo |
| 9 | Sigilo médico no acesso ao CID — NC-09 | POP-001 | Baixo |
| 10 | Citar Portaria 765/2025 — NC-10 | POPs + Guia | Baixo |
| 11 | Inserir itens numerados da NR-1 nas referências normativas | Todos | Baixo |

**Ganho de posicionamento:** as correções 3, 4 e 6 transformam o kit de "kit de riscos psicossociais" em **"o único que trata FRPRT como a NR-1 manda tratar — dentro dos fatores ergonômicos, com o critério de probabilidade do 1.5.4.4.5.3"**. Isso é diferenciação técnica verificável, não adjetivo de venda.

---

## 6. Versionamento

- **Versão nova:** `KIT_NR1_v2.0_2026-08`
- **Frase de escopo padrão para a capa:**

  > *Material elaborado conforme a NR-1, capítulo 1.5, com as redações das Portarias MTE nº 1.419, de 27/08/2024, e nº 765, de 15/05/2025 — vigente desde 26/05/2026. Documento editável, de aplicação e responsabilidade do usuário. Não substitui avaliação por profissional legalmente habilitado.*

- **Histórico de alterações** de 1 página no kit, listando as 10 correções.

---

## 7. Pendente — página de vendas

`nr1.valeriamoura.com` está bloqueada pelo proxy de rede deste ambiente; não consegui auditar. Cole o texto da página que eu verifico contra o kit real:

- datas e prazos (têm que bater com 26/05/2026)
- quantidade de arquivos prometida × 37 entregues (o COMECE_POR_AQUI diz "36 arquivos" + ele próprio — defensável, mas escolha um número e use o mesmo na página)
- garantias, promessas de atualização e de suporte
- alegações numéricas sobre multas e valores
- promessa de conformidade garantida — se houver, é exposição, porque conformidade depende da aplicação pelo cliente

---

## 8. Auditoria nº 02 — ISO 9001

Sem alteração: a ISO 9001:2026 chegou a FDIS em abril/2026 e a publicação segue prevista para **setembro/2026**, com transição até setembro/2029. Gatilho é a publicação. Estrutura pode ser preparada antes; redação normativa, não.

---

## Fontes

- NR-1 consolidada, texto atualizado 2025 (arquivo fornecido) — itens 1.5.3.1.4, 1.5.3.2.1, 1.5.4.4.5.3, 1.5.7.3.2 e 1.5.7.3.3.1
- [Portaria MTE nº 1.419/2024 (gov.br)](https://www.gov.br/trabalho-e-emprego/pt-br/assuntos/inspecao-do-trabalho/seguranca-e-saude-no-trabalho/sst-portarias/2024/portaria-mte-no-1-419-nr-01-gro-nova-redacao.pdf)
- [Portaria MTE nº 765/2025 — prorrogação da vigência (Senior)](https://documentacao.senior.com.br/exigenciaslegais/noticias/trabalhista-previdenciaria/2025/2025-05-16-prorrogacao-riscos-psicossociais/)
- [MTE prorroga gestão dos riscos psicossociais para maio de 2026 (CBIC)](https://cbic.org.br/relacoestrabalhistas/radar-trabalhista-mte-prorroga-gestao-dos-riscos-psicossociais-para-maio-de-2026/)
- [ISO 9001:2026 já passou de FDIS (facilita.etc)](https://facilita.etc.br/blog/iso-9001-2026-fdis-o-que-fazer-antes-de-setembro.html)
- [ISO 9001:2026 — orientações para a transição (SGS)](https://www.sgs.com/pt-br/showcases/iso-9001-2026-principais-atualizacoes-e-orientacoes-para-a-transicao)
