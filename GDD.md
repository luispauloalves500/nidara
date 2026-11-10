# NÍDARA — Documento de design

Baía do Véu. Um fóssil vivo nasce sem mandíbula. A dieta escreve o corpo. Três enxertos depois, a fenda acorda o Irmão Cego.

Este texto é a fonte do jogo. A versão jogável está na própria baía, no dossiê da tela inicial.

## Alto conceito

Nídara não sobe de nível. Come, e o que come abre uma porta morfológica: mandíbula, véu, cauda, serra, couraça, arco, asa, lanterna ou chifre. O poder do botão muda de verbo. Os passivos anteriores ficam.

O antagonista não é um caçador humano. É outro fóssil, que escolheu couraça em vez de sentido.

## O que isto não é

| Referência de tubarão-vingança | Nídara |
| --- | --- |
| Filhote e vingança contra um pescador | Proto-tubarão sem boca; o chefe é um parente |
| Mutações em slots sobre a mesma mordida | Um enxerto por estágio; E muda de função |
| Baía aberta enorme | Quatro anéis, uma maré, feita para o navegador |
| Humanos como eixo | Mergulhador e barco são memória, não o enredo |
| XP genérico | Carne, lume e memória — portas de dieta |

## Pilares

- O corpo é o menu.
- A dieta é a chave.
- Um botão, muitos animais.
- Uma baía, uma câmera atrás do focinho, uma maré de oito a quinze minutos.

## Loop

Berçário (sardinha no contato) → primeiro enxerto aos 90 de carne, três portas abertas → recife → segundo enxerto aos 240, com fechaduras → canal → terceiro aos 520 → Irmão Cego na fenda. Morrer encerra a maré. O recorde fica no navegador.

## Controles

Câmera de perseguição. Com o focinho à frente: A vira à esquerda, D à direita.

- W ou seta ↑ acelera. S ou seta ↓ recua.
- A ou seta ← esquerda. D ou seta → direita.
- R levanta o focinho. F abaixa.
- Espaço morde. E é o poder do último enxerto (sonar, antes do primeiro).
- Toque: alavanca, Morder, Poder, Subir, Descer.
- Controle: analógico esquerdo move, direito inclina, botão sul morde, leste usa o poder.

## Baía do Véu

Tigela. Centro fundo, borda rasa.

- Berçário, raio > 150.
- Recife, 100–150.
- Canal, 48–100.
- Fenda, < 48. Sem enxerto, a pressão mata.

## Enxertos

1. Aos 90: Fauces primevas, Véu de lume, Esporão de cauda. Todos abertos.
2. Aos 240: Serra (Fauces ou 18 presas), Couraça (1 caçador), Arco (24 de lume).
3. Aos 520: Asa (sempre), Lanterna (Véu ou 40 de lume), Chifre (Couraça ou 2 caçadores).

Se nenhuma porta abrir, o Instinto bruto empurra a maré. E segue o último enxerto. O resto vira passivo.

## Essências e presas

Carne abre o próximo corpo e aumenta o tamanho. Lume vem de água-viva. Memória vem de mergulhador ou barco destruído.

Sardinha 4 (contato). Atum 14 (mordida; contato se já houver Fauces). Foca 28. Água-viva 10 + 8 lume (contato fere; com Arco, alimenta). Mergulhador 22. Barco 36. Rival 40. Irmão 120.

## Irmão Cego

Nasce quando o terceiro enxerto fecha. Pálido, couraça, chifre, investida em linha. Matá-lo é a vitória da maré. Dá para continuar na baía depois.

## Sensação e áudio

Mandíbula, partículas, hitstop curto, tremor de câmera ao quadrado com interruptor. Áudio sintetizado, acordado no primeiro gesto, com volume e mudo. Menos movimento do sistema desliga o tremor.

## Técnico

Three.js, passo fixo em 1/60, câmera com seguimento exponencial, geometria procedural. Sem servidor de partida: save em `localStorage` (`nidara-save-v1`). O jogo cabe numa página estática — o contrato de um host como GitHub Pages.

Fora desta versão: várias baías, voz, multijogador, slots simultâneos de mutação.
