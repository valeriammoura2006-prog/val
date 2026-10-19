# Auditoria de pixels Meta — 19/10/2026

Fonte: Meta Ads (Events Manager via API), últimos 28 dias.

## Inventário
- BM "Valéria Mendes 1": 100 pixels (teto da Meta por BM)
- BM "Cuidados com a Pele": 10 pixels, todos mortos (4 nunca dispararam)
- Conta 1514071039128369: "Remarketing Qualidade" nunca disparou

## Problema 1 — CAPI (servidor) parado, navegador ativo
Sete pixels pararam de receber eventos do servidor entre 30/05 e 11/06/2026, o que sugere uma causa única (token/integração):
- SOC 2 INGLES (30/05), ATENÇÃO BÁSICA 2025 (02/06), ALBERGUE ESPANHOL (04/06), EXTERIOR ESP 2025 (05/06), PIXEL TI INGLES (06/06), 45001 ESP (08/06), FACILITIES ESPANHOL (10/06), COMERCIAL ESPANHOL (11/06)
Mais antigos:
- PIXEL QUALIDADE ALIMENTÍCIO (25/03), PIXEL FACILITIES (01/04), PIXEL COMERCIAL (15/04)
- CCIH 2026: nunca recebeu servidor
- JURÍDICO: servidor parado desde 05/10

## Problema 2 — Purchase em triplicidade (ONA)
- Cada venda chega como 1 evento do navegador + 2 do servidor (provável: CAPI nativa da Hotmart + outra integração)
- Se os event_id não forem iguais, a Meta conta compra em dobro → ROAS inflado e otimização errada

## Problema 3 — match quality baixo
- ISO 9001 2025: EMQ 6.1, sem fbc (clique do anúncio não chega), ProductPage com EMQ 3
- ONA: Purchase EMQ 9.3 (referência), topo do funil com email/telefone só em 1,2%

## Pixels mortos (+90 dias sem eventos)
Rosa Amazônica, PIXEL HOTELARIA, E-book Produtividade, RDC 63 2025, PIXEL CCIH, PIXEL ESTÉTICA, PACK ISO 2025, CAPS AD 2025 (23/07)

## Pendente
- Ler os posts https://www.instagram.com/p/Der2No_oHim/ e https://www.instagram.com/p/Dekgb1uBH6q/ (Instagram está bloqueado na rede da sessão; precisa de print ou da legenda)
