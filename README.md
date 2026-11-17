# Candidatura Automática - Skill para a IA se candidatar a vagas por você

Uma skill que ensina a IA (Claude com navegador) a se candidatar a vagas **por você** no LinkedIn (candidatura simplificada) e na Gupy: ela busca vagas que combinam com o seu perfil, escolhe a versão certa do currículo, responde os formulários só com informações verdadeiras e te entrega uma planilha com tudo o que foi enviado e o que ficou pendente.

Criada por **Joseph Santos**, especialista em recrutamento e seleção.

## O que a skill faz

1. Monta a sua **ficha de candidato** (cargo, pretensão, cidades, idiomas, ferramentas...).
2. Usa a versão certa do seu currículo para cada área.
3. **Busca vagas** compatíveis no LinkedIn e na Gupy e pula as que não combinam.
4. **Se candidata**, uma por uma, respondendo com a sua ficha.
5. Registra tudo e entrega uma **planilha**: enviadas, pendentes (o que você precisa fazer) e pontos de atenção.

**Ela nunca inventa informação, não digita senha e não aceita termos sem a sua autorização.** Quando falta algo, ela pergunta ou deixa a vaga como pendente.

## O que você precisa

- **Claude com acesso ao navegador**, por exemplo a extensão [Claude in Chrome](https://claude.com/chrome) ou o Claude Code com o Chrome conectado.
- Estar **logado** no LinkedIn e na Gupy no seu Chrome (você mesmo faz o login).
- Um **currículo pronto**. Para fazer o seu no padrão que passa nos filtros, use a skill gratuita [Currículo Aprovado](https://github.com/joseeph-cv/curriculo-aprovado-skill).

## Como usar

### Claude Code
```bash
git clone https://github.com/joseeph-cv/candidatura-automatica-skill ~/.claude/skills/candidatura-automatica
```
Depois peça: *"Se candidata a 20 vagas de Analista de Dados Júnior em São Paulo por mim"* e mande o currículo.

### Claude.ai (site ou app)
Em **Configurações > Capacidades > Skills**, envie esta pasta compactada em `.zip`. Use junto com a extensão Claude in Chrome.

### Primeira vez
Preencha a [ficha do candidato](docs/FICHA_DO_CANDIDATO.md) e mande junto com o currículo. Quanto mais completa, menos a IA para para perguntar.

## Arquivos

| Arquivo | Para que serve |
|---|---|
| [SKILL.md](SKILL.md) | As instruções da skill (o "cérebro") |
| [docs/FICHA_DO_CANDIDATO.md](docs/FICHA_DO_CANDIDATO.md) | Modelo da ficha com as respostas padrão dos formulários |
| [modelo/log_candidaturas.csv](modelo/log_candidaturas.csv) | Modelo do registro de candidaturas |

## Avisos importantes

- **Você é responsável pelas candidaturas enviadas.** Confira a planilha no final de cada rodada.
- Automatizar ações em sites pode ir contra os termos de uso de algumas plataformas. Use em ritmo humano, com poucas dezenas de vagas por rodada, e por sua conta e risco.
- A IA pode errar. Comece com uma rodada pequena (5 vagas) e acompanhe.
- Seus dados ficam no seu navegador e na IA que você usa. Confira a política de privacidade da ferramenta.

## Licença

[MIT](LICENSE): use, adapte e compartilhe à vontade, mantendo o crédito.
