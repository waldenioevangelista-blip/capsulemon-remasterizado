# Capsulemon Remasterizado

Projeto de reimplementação limpa ("clean-room") de um jogo de combate por turnos com movimentação por estilingue, colisões, dano por impacto e IA.

## Estado atual

- **V0.4.1 — Movimento:** aprovado em teste.
- **V0.5 — Colisões:** fase atual de validação.
- Protótipo atual: `prototype/v0.5.html`.

## Regras já aprovadas

- Seleção independente de P1 e P2.
- Clique/toque na unidade, puxar para trás e soltar para lançar.
- Força proporcional ao arrasto.
- Trajetória prevista durante a mira.
- Ricochete em paredes e obstáculos.
- Atrito e desaceleração.
- Turno termina somente quando todas as unidades param.
- Colisão aliada transfere impulso e não causa dano.
- Colisão contra inimigo causa dano baseado na intensidade do impacto.
- Um contato contínuo não pode aplicar dano repetido a cada frame.
- Unidade com 0 HP é eliminada da física e da seleção.

## Estrutura

```
prototype/
  v0.5.html
docs/
  MECANICAS_APROVADAS.md
  ROADMAP.md
  TESTES_V0.5.md
CHANGELOG.md
.gitignore
```

## Diretriz do projeto

O projeto não reutiliza código, sprites, áudio ou outros assets proprietários do jogo de referência. A meta é reconstruir as mecânicas com código e identidade próprios.

## Próxima etapa

Validar V0.5:
1. colisão aliada;
2. colisão inimiga;
3. impacto lateral;
4. ricochete;
5. transferência de impulso;
6. bloqueio de dano duplicado.

Depois da aprovação, seguir para combo/ataque cooperativo.
