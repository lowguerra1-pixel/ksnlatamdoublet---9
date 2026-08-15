# PV Nervio Vago — Teste de Ticket $9 / $19

Página de vendas estática (ES/LATAM) da oferta **Kit de Regulación del Sistema Nervioso**.

Variante do teste de ticket: **2 cards, $9 / $19 USD**.

| Item | Valor |
|---|---|
| Estrutura | 2 cards — Esencial + Completo |
| Plan Esencial | $9 USD (riscado $37) |
| Kit Completo | $19 USD (riscado $97) |
| Checkout Esencial | `https://go.centerpag.com/PPU38CQFCNN` |
| Checkout Completo | `https://go.centerpag.com/PPU38CQF340` |


## Os dois planos

**Plan Esencial** — os 4 baralhos (+144 cartas): Mazo del Nervio Vago (64 cartas),
Cuerpo/Corazón/Mente (+40), Patrones Heredados (+40) e Grounding. Mais acesso
vitalício, entrega imediata e garantia de 30 dias.

**Kit Completo** — tudo do Esencial, mais as 2 guias, os 2 cadernos, os 6 bônus,
atualizações futuras e a comunidade. Leva o selo "Más elegido".
## Comportamento dos CTAs

O botão da hero rola até a seção `#oferta` em vez de ir direto ao checkout — o lead
passa pela pilha de valor, bônus, prova e garantia antes de ver o preço.
O CTA final também volta aos planos, já que há duas opções. Só os botões dentro de cada card vão ao checkout.

## Deploy

Site estático, sem build. É só publicar a raiz do repositório.
No Netlify: build command vazio, publish directory `.`.

## Estrutura

```
index.html      página completa
css/index.css   Tailwind compilado
js/             pixel UTMify + rastreio de UTMs
images/         74 imagens (todas locais, sem dependência externa)
```
