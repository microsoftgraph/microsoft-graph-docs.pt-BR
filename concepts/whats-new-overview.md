---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 88cb0ba1570cd0f90fe4cc199eee3ce550c17781
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42729028"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Confira os destaques das novidades do Microsoft Graph e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista completa das atualizações da API, confira o seções do artigo de [março](changelog.md#march-2020) e [fevereiro](changelog.md#february-2020) do log de alterações da API. 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.

## <a name="march-2020-new-and-generally-available"></a>Março de 2020: novo e disponível para o público geral

### <a name="reports"></a>Relatórios
O administrador de serviços do Teams e o administrador de comunicações do Teams devem ser usados como funções de usuário aceitas para permitir que os aplicativos leiam os relatórios de uso do serviço do Office 365 em nome de um usuário, como [formas de autorização delegada pelo usuário](reportroot-authorization.md). 

## <a name="march-2020-new-in-preview-only"></a>Março de 2020: novo somente para visualização

### <a name="calendar"></a>Calendário
- Use a propriedade **calendarGroupId** para obter o [grupo de calendário](/graph/api/resources/calendargroup?view=graph-rest-beta) em que um [calendário](/graph/api/resources/calendar?view=graph-rest-beta) foi criado.
- Use a propriedade **isDraft** para identificar um [evento](/graph/api/resources/event?view=graph-rest-beta) como uma reunião que o usuário atualizou no Outlook, mas não enviou para atualizar os participantes.

### <a name="identity-and-access"></a>Identidade e acesso
Use a `PrivilegedAccess.Read.AzureResources` permissão no nível do aplicativo para [PIM (gerenciamento de identidades privilegiadas) dos recursos do Azure](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta), para configurar o fluxo de trabalho de acesso just-in-time para funções de infraestrutura do Azure em um grupo de gerenciamento, assinatura, grupo de recursos ou nível de recurso.

### <a name="teamwork"></a>Trabalho em equipe
Use a `ChannelMessage.Read.All` permissão no nível do aplicativo para ler [instâncias de](/graph/api/resources/chatmessage?view=graph-rest-beta)chatMessage em canais sem um usuário conectado.

## <a name="february-2020-new-and-generally-available"></a>Fevereiro de 2020: novo e disponível para o público geral

### <a name="calendar"></a>Calendário
Vamos examinar um exemplo de [criação de um evento em um calendário compartilhado ou delegado](outlook-create-event-in-shared-delegated-calendar.md), além das ações e propriedades disponíveis para o representante, os convidados e o proprietário do calendário durante esse processo.

### <a name="identity-and-access"></a>Identidade e acesso
- Para aumentar a segurança ao assinar as [notificações de alteração dos dados do usuário](webhooks.md), [impor o Protocolo TLS 1.2](https://docs.microsoft.com/configmgr/core/plan-design/security/enable-tls-1-2) ou mais recente em clientes e servidores de sites usados no processo de notificação. O novo requisito será lançado em estágios a partir de 15 de fevereiro de 2020. A partir de 15 de maio de 2020, todos os pontos de extremidade de notificação devem atendem ao novo requisito de TLS. [Descubra os estágios do lançamento](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) e, se necessário, use a nova propriedade **latestSupportedTlsVersion** como uma solução alternativa temporária para evitar falhas de assinatura antes de concluir a atualização de TLS.
- Use os respectivos tipos de [solicitação de avaliação de ameaças](/graph/api/resources/threatAssessmentRequest?view=graph-rest-1.0) para controlar as ameaças de [email](/graph/api/resources/mailassessmentrequest?view=graph-rest-1.0), um [arquivo de mensagem de email](/graph/api/resources/emailfileassessmentrequest?view=graph-rest-1.0) (arquivo .EML), [arquivo de anexo de email](/graph/api/resources/fileassessmentrequest?view=graph-rest-1.0) (texto, Word ou arquivo binário) ou [URL](/graph/api/resources/urlassessmentrequest?view=graph-rest-1.0).

### <a name="users"></a>Usuários
[Reprocessar](/graph/api/user-reprocesslicenseassignment?view=graph-rest-1.0) todas as atribuições de licença baseadas em grupo para um [usuário](/graph/api/resources/user?view=graph-rest-1.0).


## <a name="february-2020-new-in-preview-only"></a>Fevereiro de 2020: nova somente para visualização

### <a name="calendar"></a>Calendário
Confira [tarefas com suporte por APIs de visualização que gerenciam o compartilhamento de calendários e a delegação](outlook-share-or-delegate-calendar.md).

### <a name="cloud-communications"></a>Comunicações na nuvem

- Use o novo recurso [registros de chamadas](/graph/api/resources/callrecord?view=graph-rest-beta) para obter metadados de chamadas e reuniões online do Microsoft Teams e do Skype for Business para uma organização.
- Para um participante de uma reunião, use a propriedade **Iniciador** para obter as informações de identidade do iniciador de uma [gravação](/graph/api/resources/recordinginfo?view=graph-rest-beta), se houver uma.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [fevereiro](changelog.md#february-2020) do Intune.

### <a name="groups"></a>Grupos
Use o método [assignLicense](/graph/api/group-assignlicense?view=graph-rest-beta) para atribuir licenças de produtos, como o Office 365 ou o Enterprise Mobility + Security, a um grupo. Como o Azure AD garante que as licenças sejam designadas para os membros do grupo, os membros que ingressarem ou saírem de um grupo não precisarão mais de gerenciamento de licenças no nível individual.

### <a name="identity-and-access"></a>Identidade e acesso
- Defina as configurações de solicitação, aprovação e revisar ao criar uma [política de atribuição de pacote](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta).
- Acessar tipos específicos de [políticas de uma organização](/graph/api/resources/policy-overview?view=graph-rest-beta) usando o `/policies`segmento URL e especificando o tipo de política. Por exemplo, uma organização pode forçar uma política a entrar automaticamente no usuário de uma sessão da Web após um período de inatividade, confira as operações CRUD para instâncias de [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-beta). Essa é um [alteração significativa](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/) para que seja mais fácil descobrir todas as políticas, agrupando todas as políticas digitadas sob o `/policies`segmento. Acesse outras políticas digitadas de uma abordagem semelhante: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-beta), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta)e [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-beta). 
- Use a permissão de nível de aplicativo e `Policy.ReadWrite.ApplicationConfiguration` delegada para operações de leitura e gravação na configuração do aplicativo [políticas](/graph/api/resources/policy-overview?view=graph-rest-beta) mencionadas no item anterior.

### <a name="teamwork"></a>Trabalho em equipe
- Use [alterar as notificações](/graph/api/resources/webhooks?view=graph-rest-beta) em todas as mensagens do canal ou em todas as mensagens de chat em uma organização.
- [Recuse](/graph/api/swapshiftschangerequest-decline?view=graph-rest-beta) uma [solicitação de troca de turnos](/graph/api/resources/swapshiftschangerequest?view=graph-rest-beta) com outro usuário em uma [equipe](/graph/api/resources/team?view=graph-rest-beta).

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

