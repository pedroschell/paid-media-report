# paid-media-report

Uma skill para o Claude Code que monta **análises estratégicas e relatórios para clientes de mídia paga** separando percepção de dado verificável.

Ela foi feita para o momento mais difícil da relação com o cliente: quando os resultados caem, ele questiona a gestão da conta e pede "soluções reais". Nessa hora, um número inventado destrói a conta inteira, porque o relatório vai para uma reunião com pessoas que podem checar.

## Os princípios

1. **Toda afirmação externa tem fonte com link.** Toda afirmação interna sai dos dados que o próprio cliente forneceu.
2. **A queixa do cliente raramente aponta a causa certa.** Antes de agir, a skill quantifica: "está chegando muito lead desqualificado" pode ser 5% do problema, enquanto 48% é lead que ninguém conseguiu contatar.
3. **A tese pode ser derrubada pela pesquisa.** Se os dados contradizem o pedido, esse é o achado mais valioso do relatório, e o usuário é avisado antes do documento ficar pronto.
4. **O difícil é dito sem acusar.** Ações que dependem do cliente entram como "decisão conjunta", nunca como cobrança.

## O que vem junto

- **`SKILL.md`:** o método, com a sequência de trabalho, a estrutura de relatório que funciona, como enquadrar más notícias e os erros que custam caro.
- **`references/checklist-analises.md`:** um menu de análises em 9 blocos (enquadramento, mercado e demanda, concorrentes, mídia paga, presença orgânica e social, reputação, oferta e preço, caminho de conversão e síntese), cada uma com fonte, custo e se dá para coletar sem acesso às contas do cliente.

## Como instalar

```bash
git clone https://github.com/pedroschell/paid-media-report ~/.claude/skills/paid-media-report
```

Peça algo como *"o cliente reclamou da queda de leads, monta uma análise para a reunião"* e a skill é acionada.

## Licença

MIT
