# Plano de testes V0.5

Execute cada teste várias vezes com P1 e P2.

| ID | Teste | Resultado esperado |
|---|---|---|
| C01 | P1 acerta P2 | Sem dano; P2 recebe impulso |
| C02 | P2 acerta P1 | Sem dano; P1 recebe impulso |
| C03 | P1 acerta E1 frontalmente | Dano + transferência de impulso |
| C04 | P2 acerta E2 frontalmente | Dano + transferência de impulso |
| C05 | Impacto muito fraco | 0 dano |
| C06 | Impacto lateral | Dano inferior ao impacto frontal equivalente |
| C07 | Unidades permanecem encostadas | Dano não repete em vários frames |
| C08 | Separar e colidir novamente | Novo dano permitido |
| C09 | Colidir com parede | Ricochete sem atravessar limite |
| C10 | Colidir com ruína | Ricochete sem ficar preso |
| C11 | Cadeia P1 → P2 → E1 | Impulso deve propagar |
| C12 | HP chega a 0 | Unidade sai da arena lógica |
| C13 | Todas as unidades param | Turno muda |
| C14 | P2 é selecionado e lançado | P2, e não P1, deve se mover |

## Ao reportar bug

Informe:
- teste;
- unidade usada;
- força aproximada;
- ponto de impacto;
- comportamento esperado;
- comportamento observado.
