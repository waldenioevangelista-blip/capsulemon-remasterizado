# Mecânicas aprovadas

## Movimento — aprovado

### Seleção
- O jogador pode escolher qualquer unidade aliada viva.
- P1 e P2 possuem estado independente.
- Selecionar uma unidade não altera a posição ou estado das demais.

### Estilingue
Fluxo:
```
selecionar unidade
→ pressionar sobre a unidade
→ puxar para trás
→ visualizar direção e força
→ soltar
→ lançar imediatamente
```

- Arrasto curto deve cancelar o movimento.
- Existe limite máximo de força.
- A unidade lançada deve ser a mesma capturada no início do arrasto.

### Movimento físico
- Atrito reduz gradualmente a velocidade.
- Paredes e obstáculos geram ricochete.
- Colisões transferem impulso.
- O turno só termina quando todas as unidades vivas estiverem paradas.

## Dano — em validação junto à V0.5

- Aliado × aliado: 0 dano.
- Inimigo × inimigo: 0 dano.
- Times opostos: dano calculado pela velocidade normal relativa do impacto.
- Impacto abaixo do limiar não causa dano.
- Um contato contínuo gera no máximo um evento de dano.
- Após separação, uma nova colisão pode gerar novo dano.
- Unidade com 0 HP deixa de participar da física e não pode ser selecionada.

## Cenário

- Grid é ferramenta temporária de teste.
- A grade deve desaparecer gradualmente conforme o cenário recebe textura.
- Elementos visuais podem evoluir sem alterar seus colliders.
- Obstáculos de teste estão sendo convertidos visualmente em ruínas/rochas.
