---
name: relatorio-estrategico-cliente
description: Use ao montar análise estratégica, diagnóstico sazonal, benchmark de concorrência ou relatório de performance para cliente de mídia paga — especialmente quando o cliente reclama de queda de resultado, questiona a gestão da conta, ou pede "soluções reais" e é preciso separar percepção de dado verificável.
---

# Relatório Estratégico para Cliente

## Princípio central

**Um número inventado destrói a conta inteira.** O cliente vai levar o relatório para uma reunião com pessoas que podem checar. Toda afirmação externa precisa de fonte verificável; toda afirmação interna precisa sair dos dados que ele mesmo forneceu.

O segundo princípio: **a queixa do cliente raramente aponta a causa certa.** O trabalho é quantificar a queixa antes de agir sobre ela.

## Quando usar

- Cliente reclama de queda de leads, vendas ou qualidade e cobra explicação
- É preciso defender a estratégia sem soar defensivo
- Pediram benchmark de concorrência ou prova de sazonalidade
- Reunião de alinhamento com stakeholders que já estão desconfiados
- Relatório mensal que precisa ir além do "aqui estão os números"

**Não usar para:** dashboard operacional recorrente, report automatizado de números sem tese.

## Menu de análises

`references/checklist-analises.md` lista as análises possíveis por bloco (mercado,
concorrência, mídia paga, reputação, preço, conversão), com fonte, custo e o
subconjunto que forma o pacote base. Consulte ao definir o escopo — este arquivo
diz **como pensar**; aquele diz **o que coletar**.

## Sequência de trabalho

### 1. Verifique suas ferramentas antes de prometer ou recusar

Antes de dizer "não consigo pesquisar isso", **confirme**. Chamar `ToolSearch` com `select:WebSearch,WebFetch` custa segundos.

Anunciar uma limitação inexistente enche o relatório de placeholders desnecessários e desperdiça a confiança do usuário. O inverso — prometer pesquisa sem ter a ferramenta — é pior.

### 2. Quantifique a queixa antes de aceitá-la

Este é o passo que mais muda o resultado. A percepção do time comercial quase nunca bate com a distribuição real.

Pegue o motivo de perda / descarte / churn e calcule o peso de cada categoria:

```
Queixa: "está caindo muito idoso e criança"
Dado:   "Não efetivo" = 87 de 1.515 = 5,7%
        "Sem retorno" = 726 de 1.515 = 47,9%
```

A queixa era real, mas correspondia a 5,7% do problema. Metade era contato não estabelecido — cadência de SDR e qualidade de telefone, não segmentação de mídia.

**Sempre cheque a consistência do preenchimento antes de confiar no dado.** Se três agentes registram zero de um motivo enquanto outro registra 235, o critério diverge entre a equipe e o dado não sustenta decisão. Diga isso explicitamente no relatório.

### 3. Deixe a tese ser derrubada pela pesquisa

O pedido original pode estar errado. Se a pesquisa contradiz a premissa, **isso é o achado mais valioso do relatório** — não um obstáculo.

Exemplo real: o pedido era provar que inverno é ruim para parque aquático. A pesquisa mostrou que a cidade turística onde o cliente fica vive seu **pico** de movimento em julho. A tese virou "a demanda está na cidade e falta oferta" — argumento muito mais forte que "esperem o verão passar".

Avise o usuário assim que descobrir, antes de escrever o documento inteiro.

### 4. Separe evidência interna de externa

| Tipo | Fonte | Como usar |
|---|---|---|
| **Interna** | Relatórios e exports do próprio cliente | Impossível de contestar. Série histórica de 12+ meses já prova sazonalidade sozinha. |
| **Externa** | Web, com link | Dá contexto de mercado e tira o foco da conta. |
| **Produto** | Site oficial do cliente | Revela lacunas que ninguém mencionou. |

**Sempre leia o site do cliente com WebFetch.** Num caso de parque aquático, a ausência de menção a água aquecida — enquanto todo concorrente de inverno tem — reposicionou a análise inteira.

### 5. Busque contexto externo que absolve sem desculpar

Fatores de mercado documentados explicam variação sem culpar ninguém. Exemplo: a Meta repassou +12,15% de PIS/Cofins e ISS ao custo de anúncios no Brasil desde 01/01/2026. Isso significa que ~12 pontos de qualquer piora de CPL YoY são tributários.

Procure sempre: mudanças de precificação de plataforma, inflação de CPM do setor, mudanças regulatórias.

### 6. Ache o concorrente que fez o movimento certo

Um caso concreto e datado vale mais que dez generalidades. O melhor benchmark tem: nome, data, o que fez, e a fala do executivo justificando.

Busque em português com termos do setor. Fontes de imprensa setorial (BrasilTuris, ND Mais, portais regionais) rendem mais que blogs de marketing.

## Estrutura que funciona

```
Sumário executivo      → tese em 1 parágrafo + 3 achados numerados
A oportunidade         → o dado que reposiciona o problema
Posicionamento         → onde o cliente ganha, não onde perde
Benchmark              → 1 caso âncora detalhado + 3 modelos resumidos
Sugestões              → blocos por esforço, com priorização por horizonte
Plano de ação          → frentes com dono e prazo
Metas                  → "de → para" com base medida
Fontes                 → todos os links, agrupados por tema
```

Se o cliente pedir "só mercado e benchmark", corte Painel/Funil/Plano e renumere.

## Enquadramento: como dizer o difícil

| Em vez de | Escreva |
|---|---|
| "O time de SDR não retorna os leads" | "71% do descarte é contato não estabelecido — cadência e SLA a destravar juntos" |
| "As campanhas estão certas, o problema é de vocês" | "O ganho está em qualificação e velocidade de contato, não em compra de mídia" |
| "O parque não tem água aquecida" | "A vantagem do parque no inverno não é a água — é o destino" |
| "O site não informa data de entrega" | "Uma data pública converte promessa longa em compromisso verificável" |

Ações do cliente ficam em uma frente separada, marcada como "decisão conjunta" ou "destravar juntos" — nunca como cobrança.

## Erros que custam caro

**Anunciar limitação sem verificar.** Verifique as ferramentas primeiro.

**Aceitar a premissa do pedido sem checar.** Se os dados contradizem, avise cedo.

**Rótulo mais categórico que o dado.** "5/8 agentes preenchendo" quando o real era "critério divergente entre 8" — o número sugeria que três não preenchiam nada. Ajuste o rótulo ao que o dado sustenta.

**Remover seção e deixar referência órfã.** Ao cortar uma seção, procure menções a ela no resto do documento e nos números que ela sustentava.

**Sumir com a fonte.** Cada afirmação externa carrega link clicável. A seção de Fontes é o que sustenta a credibilidade quando alguém questiona.

## Checklist antes de entregar

- [ ] Toda afirmação externa tem link verificável
- [ ] Site do cliente foi lido diretamente
- [ ] Motivos de perda quantificados por peso, não por percepção
- [ ] Consistência de preenchimento do CRM verificada e reportada
- [ ] Contexto de mercado (tributário, inflação de CPM) considerado no YoY
- [ ] Ao menos um benchmark com nome, data e citação
- [ ] Ações do cliente enquadradas como "juntos", não como cobrança
- [ ] Sem referência órfã a seção removida
- [ ] Rótulos de indicador conferem exatamente com o dado
