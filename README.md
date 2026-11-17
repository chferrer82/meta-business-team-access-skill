# Meta Business Team Access — Skill para Claude

Uma [skill](https://docs.claude.com/en/docs/agents-and-tools/agent-skills/overview) para o Claude que guia a inclusão de membros de equipe (social media, gestor de tráfego, voluntários) em um **Business Portfolio do Meta Business Suite** com acesso corretamente delimitado — sem entregar "Acesso total" por engano.

Feita a partir de uma configuração real para uma organização (igreja/ONG) e compartilhada para a comunidade.

## O que a skill cobre

1. **Confirmar o Business Portfolio correto** antes de qualquer alteração.
2. **Convidar pessoas com acesso parcial/básico** — nunca "Full access" no nível do Portfolio.
3. **Permissões granulares por ativo** (Página do Facebook, Instagram, conta de anúncios), com perfis prontos:
   - Social media: Conteúdo + Atividade da comunidade + Mensagens
   - Gestor de tráfego: Anúncios + Insights, e "Gerenciar campanhas" (não "Gerenciar contas de anúncios") na conta de anúncios
4. **Conta de anúncios dedicada** sem forma de pagamento até a hora de publicar.
5. **A armadilha da "Instagram-Backed Ad Account" (IGBA)** — o acesso "Full access" travado que "não pode ser alterado": causa, correção passo a passo e o que é esperado depois.
6. **Checklist de segurança** (mais de um admin, 2FA, entidades desconhecidas, nenhum membro da equipe com Full access).

## Instalação

### Claude.ai (app web/desktop)
1. Baixe a pasta [`skills/meta-business-team-access`](skills/meta-business-team-access) (ou o `SKILL.md`).
2. Compacte a pasta em `.zip`.
3. Em **Settings → Capabilities → Skills**, faça o upload do arquivo.

### Claude Code
```bash
git clone https://github.com/chferrer82/meta-business-team-access-skill.git
cp -r meta-business-team-access-skill/skills/meta-business-team-access ~/.claude/skills/
```

### Claude API / Agent SDK
Use a pasta `skills/meta-business-team-access` conforme a [documentação de Agent Skills](https://docs.claude.com/en/docs/agents-and-tools/agent-skills/overview).

## Como usar

Basta pedir ao Claude algo como:

- "Quero adicionar a nossa social media na Página e no Instagram da igreja, sem dar acesso total."
- "Como dou acesso ao gestor de tráfego só para criar campanhas?"
- "No Business Settings aparece um acesso 'Full access' que não pode ser alterado. O que é isso?"

## Aviso

A interface da Meta muda com frequência e os nomes de menu variam por idioma e região. Se algo não bater, a própria skill orienta a usar o assistente de suporte da Meta em `business.facebook.com/business/help` com os IDs relevantes. Este projeto não tem vínculo com a Meta.

## Contribuindo

Encontrou um menu com nome diferente, um caso novo ou uma correção? Abra uma *issue* ou *pull request* — veja [CONTRIBUTING.md](CONTRIBUTING.md).

## Licença

[MIT](LICENSE)

---

### English summary

A Claude skill for adding team members (social media managers, ad managers, volunteers) to a Meta Business Suite Business Portfolio with properly scoped access to a Facebook Page, Instagram account and ad account — and for diagnosing the locked "Instagram-Backed Ad Account" (IGBA) owner entity. The skill content is in Brazilian Portuguese. Install by copying `skills/meta-business-team-access` into your skills directory or uploading it as a zip in Claude.ai.
