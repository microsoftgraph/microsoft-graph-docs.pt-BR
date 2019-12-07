---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: ae0ec1d070a163cbb093dfabfb36edf2b034f441
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895490"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Confira os destaques das novidades do Microsoft Graph e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista completa de atualizações da API, confira as seções de [dezembro](changelog.md#december-2019) e [novembro](changelog.md#november-2019) do log de alterações da API. 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.


## <a name="december-2019-new-in-preview"></a>Dezembro de 2019: novidades na versão prévia

### <a name="teamwork"></a>Trabalho em equipe
- [Configure as notificações que incluem dados de recursos](webhooks-with-resource-data.md) para recursos do [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) nos canais e bate-papos do Microsoft Teams.
- [Assine as notificações](/graph/api/resources/subscription?view=graph-rest-beta) de [mensagens de canal ou de bate-papo](/graph/api/resources/chatmessage?view=graph-rest-beta) novas ou modificadas.

## <a name="november-2019-new-and-generally-available"></a>Novembro de 2019: novo e disponível para o público geral

### <a name="groups"></a>Grupos
- Use permissões delegadas ou de aplicativo, GroupMember.Read.All e GroupMember.ReadWrite.All, para listar grupos, leia as propriedades básicas do grupo, leia (e atualize a permissão de leitura/gravação) a associação dos grupos aos quais o aplicativo tem acesso.
- Use a permissão do aplicativo, Group.Create, para criar grupos sem um usuário conectado.
- Para um [grupo](/graph/api/resources/group?view=graph-rest-1.0) especificado, [verifique a associação](/graph/api/group-checkmemberobjects?view=graph-rest-1.0) em outros grupos ou funções de diretório.

### <a name="identity-and-access"></a>Identidade e acesso
- Registre [aplicativos](/graph/api/resources/application?view=graph-rest-1.0) que se autenticam com o Azure Active Directory (Azure AD). Use as [permissões](/graph/permissions-reference#application-resource-permissions) delegadas, Application.Read.All e Application.ReadWrite.All ou as permissões de aplicativos, Application.Read.All, conforme apropriado.
- Para um [dispositivo](/graph/api/resources/device?view=graph-rest-1.0) especificado, [verifique a associação](/graph/api/device-checkmemberobjects?view=graph-rest-1.0) em outros grupos ou funções de diretório.

### <a name="mail"></a>Email
- Use a propriedade **conversationIndex** para obter a posição de uma mensagem em uma conversa de email do Outlook.
- Use a permissão delegada, Mail.ReadBasic e a permissão de aplicativo, Mail.ReadBasic.All, para obter os recursos de [mensagem](/graph/api/resources/message?view=graph-rest-1.0) ou de [pasta de email](/graph/api/resources/mailfolder?view=graph-rest-1.0), acompanhar suas alterações e gerenciar [assinaturas](/graph/api/resources/subscription?view=graph-rest-1.0) para notificações de alteração nas mensagens.

### <a name="users"></a>Usuários
- [Verifique se há associações de grupo](/graph/api/user-checkmemberobjects?view=graph-rest-1.0) de um [usuário](/graph/api/resources/user?view=graph-rest-1.0) específico.
- Use a propriedade **creationType** para descobrir como uma conta de usuário foi criada, por exemplo, se a conta foi criada como uma conta corporativa ou de estudante ou como uma conta externa, etc.

## <a name="november-2019-new-in-preview"></a>Novembro de 2019: Novidades na versão prévia

### <a name="calendar"></a>Calendário
- [Use o Outlook para organizar e participar de reuniões online](outlook-calendar-online-meetings.md).
- [Defina as propriedades](/graph/api/place-update?view=graph-rest-beta) para os tipos de local avançado de [sala](/graph/api/resources/room?view=graph-rest-beta) e [lista de sala](/graph/api/resources/roomlist?view=graph-rest-beta).

### <a name="cloud-communication"></a>Comunicação na nuvem
O tipo de recurso de [chamada](/graph/api/resources/call?view=graph-rest-beta) dá suporte aos seguintes recursos adicionais:

- O [contexto de uma chamada de entrada](/graph/api/resources/incomingcontext?view=graph-rest-beta)
- O tipo de ponto de extremidade de um participante, como correio de voz ou Skype for Business
- A capacidade de [atualizar](/graph/api/call-updaterecordingstatus?view=graph-rest-beta) as [informações de registro](/graph/api/resources/recordinginfo?view=graph-rest-beta) de um [participante](/graph/api/resources/participant?view=graph-rest-beta)

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [novembro](changelog.md#november-2019) do Intune

### <a name="education"></a>Educação
Os administradores podem habilitar as configurações de toda a classe por meio da propriedade **classSettings** da [equipe](/graph/api/resources/team?view=graph-rest-beta) associada à [classe](/graph/api/resources/educationclass?view=graph-rest-beta). Atualmente, há uma configuração para notificar os guardiões sobre tarefas semanais.

### <a name="identity-and-access"></a>Identidade e acesso
- Use a permissão do aplicativo, Policy.Read.All, para ler todas as políticas de acesso condicional da sua localização e locais nomeados, sem um usuário conectado.
- Permita que a [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta) esteja em um estado somente de relatório, `enabledForReportingButNotEnforced`.
- Use a permissão delegada, ThreatAssessment.ReadWrite.All, ou a permissão de aplicativo, ThreatAssessment.Read.All, leia (ou crie uma permissão de leitura/gravação) solicitações para avaliar ameaças em uma organização.

### <a name="mail"></a>Email
Use a permissão delegada, Mail.ReadBasic e a permissão de aplicativo, Mail.ReadBasic.All, para gerenciar as [assinaturas](/graph/api/resources/subscription?view=graph-rest-beta) para notificações de alteração no recurso de [mensagem](/graph/api/resources/message?view=graph-rest-beta).

### <a name="notifications"></a>Notificações
Use as novas notificações simples [SDK Web](https://aka.ms/GNSDK) em vez do [SDK do Project Rome](https://github.com/Microsoft/project-rome), para aproveitar um modelo de autenticação aperfeiçoado e suporte a aplicativos da Web usando o push da Web. 

### <a name="people-and-workplace-intelligence"></a>Inteligência de pessoas e local de trabalho
Estreia do recurso do [perfil](/graph/api/resources/profile?view=graph-rest-beta) que é uma representação avançada da próxima geração de entidades de pessoas nos serviços da Microsoft. Esse recurso se relaciona aos atributos comuns e práticos de pessoas, incluindo informações sobre datas significativas, como [aniversários](/graph/api/resources/personanniversary?view=graph-rest-beta), [escolaridade](/graph/api/resources/educationalactivity?view=graph-rest-beta), [cargos](/graph/api/resources/workposition?view=graph-rest-beta), [interesses](/graph/api/resources/personinterest?view=graph-rest-beta), [idioma](/graph/api/resources/languageproficiency?view=graph-rest-beta) e [habilidades](/graph/api/resources/skillproficiency?view=graph-rest-beta) e competências, [participação em projetos](/graph/api/resources/projectparticipation?view=graph-rest-beta), [associação em sites](/graph/api/resources/personwebsite?view=graph-rest-beta) e outras informações de contato e [conta](/graph/api/resources/useraccountinformation?view=graph-rest-beta).

### <a name="search"></a>Pesquisar
Estreia da [API de Pesquisa da Microsoft](search-concept-overview.md) que permite aos usuários do aplicativo obter os resultados de pesquisa mais atualizados, personalizados e relevantes com a plataforma Microsoft Graph. Use o recurso de [consulta](/graph/api/search-query?view=graph-rest-beta)por padrão, pesquisas mensagens e eventos do Outlook e arquivos do OneDrive e do SharePoint na nuvem da Microsoft. Use os conectores [disponíveis](/microsoftsearch/connectors-overview) na [galeria de conectores do Microsoft Graph](/microsoftsearch/connectors-gallery), para incluir dados de pesquisa fora do Microsoft Cloud. Como alternativa, [construa seus próprios conectores](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), indexe arquivos e itens personalizados externos e consulte fontes de dados externas específicas.

### <a name="teamwork"></a>Trabalho em equipe
Obtenha os recursos de [arquivo](/graph/api/resources/driveitem?view=graph-rest-beta) associados a uma [equipe](/graph/api/resources/team?view=graph-rest-beta) e [canal](/graph/api/resources/channel?view=graph-rest-beta) usando a seguinte sintaxe de solicitação de HTTP:

```http
GET /teams/{teamId}/channels/{channelId}/filesFolder
```

### <a name="users"></a>Usuários
Use a propriedade **creationType** para descobrir como uma conta de usuário foi criada, por exemplo, se a conta foi criada como uma conta corporativa ou de estudante ou como uma conta externa, etc.

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

