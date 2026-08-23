# Checklist de análises — estudo de mercado

Menu de análises possíveis. **Não é para rodar tudo.** Escolha o recorte pelo escopo
combinado (ver "Escopos" no fim) e pelo que o negócio pede.

O `SKILL.md` diz **como pensar**. Este arquivo diz **o que coletar**.

## Duas regras que atravessam tudo

**1. Toda análise é comparativa.** Nunca "o Concorrente A tem 5 anúncios", e sim
"Concorrente A 5, o cliente 3, há 22 meses contra 5 semanas". Mapear o mercado sem
posicionar o cliente dentro dele produz relatório de leitura, não de decisão.

O cliente é uma empresa pública como as outras — site, redes, preço, anúncios ativos
e Google Meu Negócio dele são tão raspáveis quanto os dos concorrentes. **Não é
preciso pedir acesso a nada para compará-lo.**

**2. O que exige acesso fica separado.** Itens 🔒 dependem de acesso às contas ou
ao CRM do cliente. Quando esse acesso não existe, eles saem do relatório principal
e entram na seção "limites do levantamento", dizendo o que não foi medido e por quê.

## Legenda

| | Significado |
|---|---|
| 🟢 | Grátis e coletável por agente hoje |
| 🟡 | Grátis, mas manual — custa tempo humano |
| 🔒 | **Exige acesso às contas ou ao CRM do cliente** |
| 🔴 | Exige ferramenta paga (Semrush, Similarweb, Pathmatics) |

★ = entra no pacote base.

---

## Bloco 0 — Enquadramento (antes de coletar qualquer coisa)

Pular este bloco é o erro mais caro: coletar dado sobre o mercado errado.

| # | Análise | Pergunta que responde | Fonte | |
|---|---|---|---|---|
| 0.1 ★ | Definição do negócio em uma frase | O que vende, para quem, onde | Site do cliente | 🟢 |
| 0.2 ★ | Delimitação da praça | Qual o raio de atuação **real**, não o desejado | Site + Google Meu Negócio | 🟢 |
| 0.3 ★ | Ticket e modelo de receita | Recorrente ou avulso? Muda o cálculo de mercado | Preços públicos | 🟡 |
| 0.4 ★ | Lista fechada de concorrentes | Quais 3 diretos + 2 indiretos serão rastreados | Bloco 2 | 🟢 |
| 0.5 ★ | Hipótese central | O que o dado sugere ser o problema | Coleta | 🟡 |

> Em prospect frio não existe queixa — ele não contratou nada ainda. A hipótese
> nasce da coleta. **Quando já for cliente**, 0.5 vira "quantificar a queixa",
> conforme o passo 2 do `SKILL.md`, e aí é 🔒.

> A lista de concorrentes que o cliente daria estaria incompleta de qualquer jeito.
> Feche-a **depois** do Bloco 2.

---

## Bloco 1 — Mercado e demanda

| # | Análise | Pergunta que responde | Fonte | |
|---|---|---|---|---|
| 1.1 ★ | Tamanho da praça | População, domicílios, renda, frota do município | IBGE Cidades | 🟢 |
| 1.2 | Densidade de empresas do setor | Quantos concorrentes o município comporta | DataSebrae | 🟢 |
| 1.3 ★ | Sazonalidade da demanda | Quando o mercado aquece e esfria — 5 anos | Google Trends (região) | 🟡 |
| 1.4 ★ | Volume de busca comercial | Quanta gente procura ativamente | Keyword Planner / Trends | 🟡 |
| 1.5 | Tendência da categoria | O mercado cresce, estagnou ou encolhe | Trends + imprensa setorial | 🟢 |
| 1.6 ★ | Evento que muda o jogo | Regulação, tributo, entrada de player nacional | Busca web + imprensa | 🟢 |
| 1.7 | Dimensionamento aterrissado | Quantas vendas/mês o mercado local comporta | Cruzamento de 1.1–1.4 | 🟡 |

### Quem é o público

Renda e idade saem **do território (IBGE) ou da conta do cliente**. Nunca de
inferência — persona inventada é o tipo de número que destrói a conta inteira.

| # | Análise | Pergunta que responde | Fonte | |
|---|---|---|---|---|
| 1.8 ★ | Pirâmide etária e renda do município | Tem gente suficiente, e com o dinheiro certo? | IBGE Censo 2022 | 🟢 |
| 1.9 | Perfil por bairro (setor censitário) | Onde na cidade está o público que paga | IBGE | 🟢 |
| 1.10 | Perfil de quem já compra (CEP × censo) | Onde tem mais gente igual a quem já compra | Base do cliente + IBGE | 🔒 |
| 1.11 | Demografia de quem converteu | Quem realmente vira venda | Contas de anúncio | 🔒 |
| 1.12 | Tamanho de público por segmentação | Quanta gente dá para alcançar | Gerenciador de Anúncios | 🔒 |

> A API do IBGE é aberta e sem chave. **Confirme o número da tabela no SIDRA na hora
> de implementar** — muda por recorte, não afirme de memória.

> **1.6 é o item de maior retorno do bloco.** Uma lei nova que muda o setor ou um
> repasse de imposto da plataforma de anúncios (como os +12,15% da Meta no Brasil em
> 2026) explicam variações que pareciam culpa da conta. Um fato datado e verificável
> reposiciona o relatório.

---

## Bloco 2 — Quem são os concorrentes

| # | Análise | Pergunta que responde | Fonte | |
|---|---|---|---|---|
| 2.1 ★ | Mapeamento no local pack | Quem o Google mostra para quem busca na região | Google Maps / Busca | 🟡 |
| 2.2 | Mapeamento orgânico | Quem domina os termos comerciais | Busca web | 🟡 |
| 2.3 ★ | Concorrente só-mídia-paga | Quem aparece na ad library e não no Maps | Bloco 3 | 🟢 |
| 2.4 ★ | Concorrência indireta de leilão | Quem disputa a mesma impressão sem vender o mesmo | Ad libraries | 🟢 |
| 2.5 | Nacional vs regional | Quem tem foco real na praça | Cruzar busca nacional × regional | 🟢 |
| 2.6 | Porte e tempo de mercado | Com quem dá para brigar e com quem não dá | CNPJ público, redes | 🟡 |

> **2.4 é achado, não rotina.** Num cliente de turismo, bancos e incorporadoras
> anunciando o nome do destino explicavam o CPM inflado — informação que nenhum
> concorrente daria.

---

## Bloco 3 — Mídia paga (o núcleo da análise)

O bloco que ninguém entrega para negócio pequeno. Tudo público e gratuito, exceto 🔒.

### 3A — Meta (Facebook + Instagram) — skill `biblioteca-anuncios-meta`

| # | Análise | Pergunta que responde | |
|---|---|---|---|
| 3.1 ★ | Nº de anúncios ativos por concorrente | Quem investe de verdade | 🟢 |
| 3.2 ★ | Data do anúncio mais antigo | Há quanto tempo investe — separa quem testa de quem opera | 🟢 |
| 3.3 | Constância / gaps de veiculação | Campanha ligada direto ou aos trancos | 🟡 |
| 3.4 | Variações do mesmo criativo | Capacidade de teste do concorrente | 🟢 |
| 3.5 ★ | Formato dominante | Vídeo, estático, carrossel | 🟡 |
| 3.6 ★ | Oferta e ângulo do criativo | O que prometem, com que gancho | 🟡 |
| 3.7 | Destino do clique | Site, WhatsApp, formulário — revela o funil | 🟡 |
| 3.8 | Prova social no criativo | Usam depoimento, nota, número de clientes | 🟡 |

### 3B — Google (Search, YouTube, Display) — **a construir**

| # | Análise | Pergunta que responde | Fonte | |
|---|---|---|---|---|
| 3.9 ★ | Presença por superfície | Anuncia em Search? YouTube? Display? | Ads Transparency Center | 🟢 |
| 3.10 ★ | Data de início e formatos | Há quanto tempo, com que peça | Ads Transparency Center | 🟢 |
| 3.11 | Texto de anúncio de Search | Qual promessa está no leilão | Ads Transparency Center | 🟡 |

### 3C — Outros canais

| # | Análise | Cobertura BR | Fonte | |
|---|---|---|---|---|
| 3.12 | TikTok — anúncios ativos | **Verificar** (a biblioteca é focada em EEE) | TikTok Commercial Content Library | 🟡 |
| 3.13 | TikTok — criativos em alta na categoria | Boa | TikTok Creative Center | 🟡 |
| 3.14 | LinkedIn — só se B2B | Boa | LinkedIn Ad Library | 🟢 |

### 3D — Leitura cruzada

| # | Análise | Pergunta que responde | |
|---|---|---|---|
| 3.15 ★ | Share of voice por termo | Quantos anunciantes disputam cada palavra | 🟢 |
| 3.16 ★ | Termos disputados × ignorados | Onde há oceano vazio | 🟢 |
| 3.17 ★ | Quem **não** anuncia | É lead de tráfego ou vive de indicação | 🟢 |
| 3.18 | Mix de canais do concorrente | Está em 1 canal ou em 4 | 🟢 |
| 3.19 | Auction Insights / parcela de impressões | Quanto do leilão se perde e para quem | 🔒 |
| 3.20 | CPM/CPC de referência da categoria | Quanto custa entrar | 🔒🔴 |

> **Parcela de impressões não é obtível de fora.** Só existe dentro da conta, e só
> com mais de 10% de parcela na campanha. Sem acesso à conta, não prometa esse
> número: ele só existe a partir do primeiro mês de gestão.

> **3.16 é a leitura mais convincente.** "Você disputa 140 anúncios e ignora 2.360" é
> um argumento que o dono entende em cinco segundos.

---

## Bloco 4 — Presença orgânica e social

| # | Análise | Pergunta que responde | Fonte | |
|---|---|---|---|---|
| 4.1 ★ | Seguidores por rede — cliente × concorrentes | Tamanho do ativo próprio de cada um | Perfis públicos | 🟢 |
| 4.2 | Frequência de postagem | Quem mantém cadência | Perfis públicos | 🟡 |
| 4.3 | Engajamento vs benchmark da rede | O ativo é vivo ou inflado | Perfis + benchmark | 🟡 |
| 4.4 | Formato que performa | Onde o público responde | Perfis públicos | 🟡 |
| 4.5 ★ | Presença por canal | Tem TikTok? YouTube? X? Onde o cliente não está | Checagem por perfil | 🟢 |
| 4.6 ★ | Velocidade do site (PageSpeed) | Quanto se perde antes de carregar | API PageSpeed Insights | 🟢 |
| 4.7 | Posição orgânica nos termos comerciais | Precisa pagar por tudo? | Busca web | 🟡 |

> Demografia de seguidor de concorrente **não é pública** — o Insights só o dono da
> conta vê, e o Audience Insights do Facebook foi desativado. Inferir por comentário
> é ruidoso e caro. Não vire item de catálogo.

---

## Bloco 5 — Reputação e prova social

| # | Análise | Pergunta que responde | Fonte | |
|---|---|---|---|---|
| 5.1 ★ | Nota e volume no Google — cliente × concorrentes | Quem tem prova social acumulada | Google Maps | 🟡 |
| 5.2 | Recência das avaliações | A operação está viva | Google Maps | 🟡 |
| 5.3 ★ | Temas das críticas negativas dos concorrentes | **A brecha de posicionamento mais barata que existe** | Avaliações públicas | 🟡 |
| 5.4 | Reclame Aqui e taxa de resposta | Risco reputacional da categoria | Reclame Aqui | 🟢 |
| 5.5 ★ | Completude do Google Meu Negócio | Categoria, fotos, horário, posts | Google Maps | 🟡 |

> **5.3** custa pouco e paga muito: ~30 avaliações ≈ 2 mil tokens por concorrente.
> A API oficial de Places devolve só ~5 avaliações — insuficiente para achar tema
> recorrente, por isso é coleta por navegador. **Confirmar antes de codar.**

> **5.5** é o maior fator isolado de ranking no mapa local, o que pesa muito para
> negócio regional.

---

## Bloco 6 — Oferta e preço

| # | Análise | Pergunta que responde | Fonte | |
|---|---|---|---|---|
| 6.1 ★ | Tabela de preços públicos | Onde o cliente está no mapa | Sites, anúncios | 🟡 |
| 6.2 ★ | Escopo do que está incluso | Preço parecido, entrega diferente | Sites | 🟡 |
| 6.3 | Condição de entrada | Isenção, adesão, fidelidade, primeira parcela | Sites, anúncios | 🟡 |
| 6.4 | Garantia / risco reverso | Quem tira o medo da compra | Sites | 🟡 |
| 6.5 ★ | Mapa de posicionamento preço × entrega | O gráfico que mais convence numa reunião | Cruzar 6.1–6.4 | 🟡 |

---

## Bloco 7 — Caminho de conversão

Barato de coletar, quase sempre rende achado. Ninguém entrega isso nesse preço.

| # | Análise | Pergunta que responde | Fonte | |
|---|---|---|---|---|
| 7.1 ★ | Nº de passos do clique ao contato | Onde o lead evapora | Navegação manual | 🟡 |
| 7.2 ★ | Teste de mistério no WhatsApp | Em quanto tempo o concorrente responde | Contato real | 🟡 |
| 7.3 ★ | Comunicação, gatilhos e message match | A promessa sobrevive ao clique | Navegação manual | 🟡 |
| 7.4 ★ | Rastreamento instalado (pixel, GTM) | O concorrente otimiza ou está no escuro | fetch + regex | 🟢 |

> **7.2 é o achado que mais choca o cliente.** "Três dos seus quatro concorrentes
> levam mais de 6 horas para responder" vale mais que qualquer gráfico.
>
> Uma mensagem por concorrente, como interessado, é **cliente oculto** — prática
> padrão. Automatizar em volume vira disparo abusivo e derruba o número. Manual por
> decisão. Registre: hora do envio (mesma janela para todos), hora da 1ª resposta,
> humano ou bot, se pediu dado antes de atender, se houve follow-up.

> **7.4** custa uma requisição e responde se o concorrente sabe fazer remarketing.

---

## Bloco 8 — Síntese (obrigatório, sempre)

| # | Entrega | Regra |
|---|---|---|
| 8.1 ★ | **Achado central** | Uma frase, com número, que reposiciona o problema |
| 8.2 ★ | Mapa de posicionamento | Onde o cliente ganha, não onde perde |
| 8.3 ★ | 3 movimentos priorizados | Ordenados por esforço × impacto |
| 8.4 ★ | O que **não** fazer | Tão valioso quanto a recomendação |
| 8.5 ★ | Limites do levantamento | O que não foi medido e por quê |
| 8.6 ★ | Fontes com link | Toda afirmação externa é clicável |

---

## Escopos

**Base (★).** O conjunto mínimo. Todo item ★ é gratuito e coletado de fora, sem
depender de nenhum acesso do cliente.

**Completo.** Base + os 🟡 que interessam ao setor. Custa tempo humano, não dinheiro.

**Monitoramento.** Subconjunto re-rodado no tempo, mostrando movimento: 3.1, 3.2,
3.9, 3.15, 5.1, 6.1. O estudo é a foto; o monitoramento é o filme.

**Com acesso (🔒).** Exige acesso às contas ou ao CRM do cliente. Entra quando esse
acesso existe.

## O que fica de fora de propósito

| Fora | Por quê |
|---|---|
| Tráfego estimado do concorrente | Só com ferramenta paga. Impreciso em negócio pequeno. |
| Investimento em R$ do concorrente | Não é público fora de anúncio político. Chutar destrói tudo. |
| Demografia de seguidor de concorrente | Não existe publicamente. Inferir é ruidoso. |
| Pesquisa primária com consumidor | Outra metodologia, outro custo. |
| Análise de produto/feature | Vocabulário de SaaS B2B. Não se aplica ao cliente regional. |

## Antes de entregar

- [ ] Todo item ★ foi rodado ou marcado como não aplicável
- [ ] **Toda análise posiciona o cliente, não só mapeia o mercado**
- [ ] Nenhum item 🔒 apareceu sem o acesso correspondente
- [ ] Nenhum número externo sem link
- [ ] Nenhum investimento de concorrente estimado em R$
- [ ] Concorrentes do Bloco 0 conferidos contra o que o Bloco 2 achou
- [ ] Achado central cabe em uma frase e tem número
- [ ] Limites declarados: o que não foi medido e por quê
