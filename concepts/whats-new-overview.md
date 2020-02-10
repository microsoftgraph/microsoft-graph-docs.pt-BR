---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 5e56d74e35bf55caade6c0137619d0d24ecc7323
ms.sourcegitcommit: cea768f767cf27a938b72bb26892d70e3dedaf2e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/08/2020
ms.locfileid: "41865848"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Confira os destaques das novidades do Microsoft Graph e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista completa de atualizações da API, confira as seções de [dezembro](changelog.md#december-2019) e [novembro](changelog.md#november-2019) do log de alterações da API. 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.

## <a name="february-2020-new-and-generally-available"></a>Fevereiro de 2020: novo e disponível para o público geral

### <a name="calendar"></a>Calendário
Vamos examinar um exemplo de [criação de um evento em um calendário compartilhado ou delegado](outlook-create-event-in-shared-delegated-calendar.md), além das ações e propriedades disponíveis para o representante, os convidados e o proprietário do calendário durante esse processo.

### <a name="security"></a>Segurança
Para aumentar a segurança ao assinar as [notificações de alteração dos dados do usuário](webhooks.md), [impor o Protocolo TLS 1.2](https://docs.microsoft.com/configmgr/core/plan-design/security/enable-tls-1-2) ou mais recente em clientes e servidores de sites usados no processo de notificação. O novo requisito será lançado em estágios a partir de 15 de fevereiro de 2020. A partir de 15 de maio de 2020, todos os pontos de extremidade de notificação devem atendem ao novo requisito de TLS. [Descubra os estágios do lançamento](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) e, se necessário, use a nova propriedade **latestSupportedTlsVersion** como uma solução alternativa temporária para evitar falhas de assinatura antes de concluir a atualização de TLS.

## <a name="february-2020-new-in-preview"></a>Fevereiro de 2020: novidades na versão prévia

### <a name="calendar"></a>Calendário
Confira [tarefas com suporte por APIs de visualização que gerenciam o compartilhamento de calendários e a delegação](outlook-share-or-delegate-calendar.md).


## <a name="january-2020-new-and-generally-available"></a>Janeiro de 2020: Novo e disponível para o público geral

### <a name="security"></a>Segurança
Como parte do gerenciamento de alerta de cliente, use o método de [alerta de atualização](/graph/api/alert-update?view=graph-rest-1.0) e atualize o campo **comentários** como `Closed in IPC` ou `Closed in MCAS`.

### <a name="teamwork"></a>Trabalho em equipe
Use a propriedade de navegação **primaryChannel** de uma [equipe](/graph/api/resources/team?view=graph-rest-1.0) para acessar o canal padrão, **Geral**.

### <a name="users"></a>Usuários
Use a propriedade **identities** para acessar uma ou mais identidades que um [usuário](/graph/api/resources/user?view=graph-rest-1.0) pode usar para entrar em uma conta de usuário do Azure AD. As identidades podem ser fornecidas pela Microsoft, por organizações ou por provedores de identidade social, como Facebook, Google ou Microsoft. Essa propriedade permite que o usuário entre na conta de usuário com uma dessas identidades.

## <a name="january-2020-new-in-preview"></a>Janeiro de 2020: novidades na versão prévia

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [janeiro](changelog.md#january-2020) do Intune.

<!--
### Identity and access
Access specific types of [policies for an organization](/graph/api/resources/policy-overview?view=graph-rest-beta) using the `/policies` URL segment and specifying the policy type. For example, an organization can enforce a policy to automatically sign a user out from a web session after a period of inactivity; see CRUD operations for instances of [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-beta). This is a [breaking change](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/) to make it easier to discover all policies, by grouping all typed policies under the `/policies` segment. Access other typed policies in a similar approach: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-beta), and [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta).
-->


## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de visualização **_prévia_**. As atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de**_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Office 365](https://developer.microsoft.com/office/dev-program), obtenha uma assinatura gratuita do Office 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).

