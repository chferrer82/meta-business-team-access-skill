---
name: meta-business-team-access
description: >
  Adicionar membros de equipe (social media, gestor de tráfego/ads, voluntários etc.)
  a um Business Portfolio do Meta Business Suite com acesso corretamente delimitado a
  uma Página do Facebook, conta do Instagram e/ou conta de anúncios — sem dar acesso
  total (Full Access) por engano. Cobre também a criação de uma conta de anúncios
  dedicada e o diagnóstico/correção da armadilha comum da "Instagram-Backed Ad Account"
  (conta de anúncios travada, criada automaticamente, aparecendo como "Full access...
  não pode ser alterado"). Acionar sempre que o usuário quiser convidar alguém para
  gerenciar uma Página, conta do Instagram ou conta de anúncios no Meta Business Suite,
  quiser limitar o que um membro da equipe pode fazer, estiver configurando anúncios
  para uma organização pela primeira vez, ou relatar que o Instagram/Business Settings
  mostra um acesso que "não pode ser alterado".
---

# Meta Business Suite: adicionando membros de equipe com acesso delimitado

## 1. Confirme primeiro o Business Portfolio correto
Antes de qualquer alteração, verifique em Business Settings qual Business Portfolio
está aberto (nome, ID) e confirme com o usuário que é o correto. Erros de portfólio
são difíceis de desfazer depois.

## 2. Convide a pessoa com acesso "Básico/Parcial" (nunca "Full access/Everything" no nível do Portfolio)
Business Settings → Usuários → Pessoas → Adicionar pessoas → e-mail da pessoa →
selecione "Acesso parcial/básico" (Partial/Basic access), nunca "Acesso total"
(Full access/Admin) no nível do Business Portfolio. Full access no Portfolio permite
remover outros admins (inclusive o proprietário) e excluir o negócio inteiro — por
isso deve ser evitado para papéis como social media manager ou gestor de tráfego.

## 3. Atribua cada ativo (Página, Instagram, conta de anúncios) com permissões granulares
Depois de convidado, vá em cada ativo (Página / Conta do Instagram / Conta de
anúncios) → People/Pessoas → adicione a pessoa → escolha permissões granulares,
NUNCA o toggle "Full access/Everything":

- **Página do Facebook**: ative apenas o necessário — Conteúdo, Atividade da
  comunidade, Mensagens e chamadas, Anúncios, Insights — conforme o papel.
  Social media manager: Conteúdo + Atividade da comunidade + Mensagens.
  Gestor de tráfego: Anúncios + Insights.
- **Conta do Instagram**: mesma lógica — Conteúdo, Atividade da comunidade,
  Mensagens, Anúncios, Insights, Leads, Conteúdo de criador — sem marcar
  "Full access".
- **Conta de anúncios**: use "Manage campaigns (ads)" (gerenciar campanhas) —
  permite criar/editar anúncios, ver relatórios e usar o Creative Hub — e NÃO
  "Manage ad accounts" (gerenciar contas de anúncios), que dá controle
  financeiro/forma de pagamento e poder de gerenciar permissões da própria
  conta de anúncios. Esse é o nível mínimo necessário para um gestor de
  tráfego criar e rodar campanhas.

Importante: enquanto o convite da pessoa ainda estiver em status "Convidado"
(Invited, não aceito), as atribuições de ativos podem não aparecer na lista de
"People" do ativo mesmo tendo sido salvas com sucesso. Isso é esperado — não é
erro. A atribuição aparece quando a pessoa aceitar o convite.

## 4. Configure uma conta de anúncios dedicada (sem forma de pagamento ainda)
Pode-se criar e deixar uma conta de anúncios nova (ex.: "BM [Nome da
Organização]") sem forma de pagamento cadastrada. A conta funciona normalmente
para criar campanhas/conjuntos de anúncios/anúncios em rascunho com saldo R$0.
A Meta só bloqueia quando a campanha for efetivamente publicada/gastar
dinheiro — então é seguro deixar sem pagamento até os anúncios estarem prontos
para ir ao ar.

## 5. A armadilha da "Instagram-Backed Ad Account" (IGBA)
**Sintoma**: Business Settings mostra uma entidade "proprietária" (owner) com
"Full access" travado, que não pode ser editado nem removido, vinculada a uma
conta de anúncios desconhecida/não reconhecida.

**Causa**: é um sistema legado da Meta. Acontece quando um perfil profissional
do Instagram foi usado para "Impulsionar publicação" (Boost Post) direto pelo
app, antes de o Instagram estar conectado a um Business Portfolio. Isso cria
automaticamente uma entidade de "proprietário" travada e uma conta de anúncios
oculta, não gerenciável pelas configurações normais de Business Settings.

**Correção**:
1. Business Settings → Contas → Contas do Instagram → botão "+ Adicionar" →
   "Adicionar conta do Instagram".
2. Isso abre uma janela de login — a própria pessoa (dono da conta) deve
   fazer login ali com usuário/senha do Instagram (nunca digite credenciais
   de terceiros por ela).
3. Confirmar a conexão quando solicitado.
4. Isso eleva o acesso do verdadeiro proprietário em Business Settings para
   "Full access" genuíno e editável. A entidade legada antiga permanece na
   lista como um placeholder permanente — isso é esperado, por design da
   Meta, e não indica que algo falhou. Não tente remover e readicionar a
   conta do Instagram para "corrigir" isso; não resolve e pode quebrar a
   conexão.
5. Depois de reconectado: no app do Instagram → perfil → Ferramentas de
   anúncios (Ad tools) → Configurações de pagamento → selecione a nova conta
   de anúncios dedicada como padrão, para redirecionar gastos futuros para
   fora da conta de anúncios legada (IGBA).

Se os nomes de menu não corresponderem exatamente ao que está documentado aqui
(a interface da Meta muda com frequência e varia por idioma/região), use o
assistente de suporte com IA da própria Meta em
business.facebook.com/business/help, descrevendo: ID do Business Portfolio,
ID da Página, ID da conta do Instagram, ID da conta de anúncios desconhecida,
e o sintoma exato. Ele consegue diagnosticar esse cenário específico quando
recebe esses detalhes técnicos.

## 6. Checklist rápido de segurança/topologia
- Existe mais de um admin genuíno do Business Portfolio (evitar ponto único
  de falha)?
- 2FA ativado na conta pessoal do proprietário?
- Existe alguma entidade com "Full access" que ninguém reconhece? Investigar
  antes de prosseguir (pode ser outro caso de IGBA ou um convite antigo
  esquecido).
- Cada conta de anúncios pertence claramente a um único Business Portfolio —
  evitar misturar contas de anúncios entre negócios diferentes.
- Nenhum membro de equipe (social media, gestor de tráfego) tem "Full
  access" em nenhum nível — nem Portfolio, nem ativo individual, nem conta
  de anúncios.
