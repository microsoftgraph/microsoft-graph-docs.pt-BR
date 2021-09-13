---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 8935a5e0cc075fb88ea39fa6390be49a52a68f25
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59133972"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Recursos, incluindo APIs e ferramentas, no status de _visualização_ podem mudar sem aviso prévio e alguns podem nunca ser promovidos ao status de disponibilidade geral (GA). Não utilize recursos de visualização em aplicativos de produção.

## <a name="august-2021-new-and-generally-available"></a>Agosto de 2021: novo e geralmente disponível

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações mensais do Intune para a versão v1.0. Defina o filtro de **Data** para agosto de 2021 e procure uma seção com este mesmo cabeçalho.

### <a name="devices-and-apps--service-health-and-communications"></a>Dispositivos e aplicativos | Integridade do serviço e comunicações
GA da [API de comunicações de serviço](service-communications-concept-overview.md) no Microsoft Graph para acessar o status de integridade e as postagens do centro de mensagens sobre os serviços em nuvem da Microsoft.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Obtenha uma coleção de escopos de revisão de acesso usados para definir revisores e revisores substitutos para uma [instância de revisores de acesso](/graph/api/resources/accessReviewInstance).

## <a name="august-2021-new-in-preview-only"></a>Agosto de 2021: novo apenas em visualização

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações mensais do Intune para a versão beta. Defina o filtro de **Data** para agosto de 2021 e procure uma seção com este mesmo cabeçalho.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- [Reprocesse](/graph/api/accesspackageassignmentrequest-reprocess?view=graph-rest-beta&preserve-view=true) uma [solicitação de atribuição de pacote de acesso](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true) para repetir automaticamente a solicitação de acesso de um usuário ao pacote.
- [Reprocesse](/graph/api/accesspackageassignment-reprocess?view=graph-rest-beta&preserve-view=true)[ uma atribuição de pacote de acesso](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true) para reavaliar e impor automaticamente as atribuições de um usuário.
- [Obtenha um conjunto de requisitos de política](/graph/api/accesspackage-getapplicablepolicyrequirements?view=graph-rest-beta&preserve-view=true) para criar uma [solicitação de atribuição para um pacote de acesso](/graph/api/resources/accesspackageassignmentrequestrequirements?view=graph-rest-beta&preserve-view=true).
- Obtenha uma coleção de recursos de [revisão de acesso](/graph/api/resources/accessreviewreviewer?view=graph-rest-beta&preserve-view=true) que é usada para definir revisores contatados para uma [instância de revisores de acesso](/graph/api/resources/accessReviewInstance?view=graph-rest-beta&preserve-view=true).
- Obtenha ou defina a duração de inatividade a partir da qual as recomendações são definidas nas [configurações de agendamento de uma revisão de acesso](/graph/api/resources/accessReviewScheduleSettings?view=graph-rest-beta&preserve-view=true) usando a propriedade **RecommendationLookBackDuration**.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- As organizações podem usar [políticas para aplicar as melhores práticas para aplicativos usando métodos de autenticação de aplicativos](/graph/api/resources/applicationauthmethodpolicy?view=graph-rest-beta&preserve-view=true). Essas políticas podem ser aplicadas a [aplicativos e entidades de serviço específicos](/graph/api/resources/appmanagementpolicy?view=graph-rest-beta&preserve-view=true) ou a [todos os aplicativos e entidades de serviço em um locatário](/resources/tenantappmanagementpolicy?view=graph-rest-beta&preserve-view=true).
- Suporte para paginação na propriedade de navegação **appRoleAssignments** para [usuários](/api/user-list-approleassignments?view=graph-rest-beta&preserve-view=true), [grupos](/api/group-list-approleassignments?view=graph-rest-beta&preserve-view=true) e [entidades de serviço](/api/serviceprincipal-list-approleassignments?view=graph-rest-beta&preserve-view=true).

## <a name="july-2021-new-and-generally-available"></a>Julho de 2021: Novo e disponível para o público em geral

### <a name="cloud-communications--calls"></a>Comunicações na nuvem | Chamadas
Suporte para um limite de capacidade para o número de participantes que um aplicativo pode controlar ao [atender](/graph/api/call-answer) uma [chamada](/graph/api/resources/call), em organizações que adotam [gravação baseada em políticas do Teams](/microsoftteams/teams-recording-policy).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- GA de provedores de identidade que compartilham um tipo de base comum [identityProviderBase](/graph/api/resources/identityproviderbase):
  - Provedores de identidade internos para cenários do Azure AD B2B em um locatário do Azure AD. Esses provedores podem oferecer suporte ao Azure AD, conta Microsoft (MSA) ou senhas únicas de email.
  - Provedores de identidade social em um locatário do Azure AD B2C para permitir que os usuários se inscrevam e entrem no serviço usando uma conta de mídia social, como Microsoft, Google, Facebook, Amazon, LinkedIn ou Twitter.
- Descontinuação da API do [provedor de identidade](/graph/api/resources/identityprovider) anterior.

### <a name="users"></a>Usuários
Permitir que um usuário [altere sua própria senha](/graph/api/user-changepassword) sem exigir uma função de administrador.


## <a name="july-2021-new-in-preview-only"></a>Julho de 2021: Novo somente para visualização

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | PC na nuvem
Uma [verificação de integridade](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) de conexão local pode identificar mais alguns tipos de erros de verificação de integridade:
- A conta do computador do PC na Nuvem não foi encontrada na unidade organizacional (`adJoinCheckComputerObjectAlreadyExists`).
- O objeto do PC na Nuvem não foi encontrado no Microsoft Azure Active Directory (`azureAdDeviceSyncCheckDeviceNotFound`).
- Tempo limite para verificar se um objeto do PC na nuvem foi sincronizado com o Microsoft Azure Active Directory (`azureAdDeviceSyncCheckLongSyncCircle`). 

Consulte a [referência](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true#cloudpconpremisesconnectionhealthcheckerrortype-values) para obter detalhes e as ações corretivas recomendadas.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações mensais do Intune para a versão beta. Defina o filtro de **Data** para julho de 2021 e procure uma seção com este mesmo título.

### <a name="devices-and-apps--multi-tenant-management"></a>Dispositivos e aplicativos | Gerenciamento de vários locatários
Lançamento da [API do Microsoft 365 Lighthouse](managedtenants-concept-overview.md) que permite que os Provedores de Serviços Gerenciados (MSPs) gerenciem remotamente vários locatários de clientes em escala para conformidade e detecção de ameaças, e ajudam a manter os dispositivos dos locatários em um estado íntegro e seguro.

### <a name="education"></a>Educação
- Obtenha uma contagem de erros e uma mensagem de status como parte do [status de uma sincronização de dados escolares](/graph/api/resources/educationsynchronizationprofilestatus?view=graph-rest-beta&preserve-view=true).
- Obtenha `extracting` ou `validating` como possíveis estados de tal sincronização.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Obtenha uma coleção de erros no ciclo de vida de uma [instância de revisão de acesso](/graph/api/resources/accessreviewinstance?view=graph-rest-beta&preserve-view=true).

### <a name="search"></a>Pesquisa
- Use a [API de Pesquisa da Microsoft para recuperar informações sobre as pessoas](search-concept-person.md) que são mais relevantes para um usuário. A relevância é determinada pelos padrões de comunicação, colaboração e pelas relações comerciais do usuário. 
- Acesse a [API de indexação de conectores](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true) no sub-namespace microsoft.graph.externalConnectors.

### <a name="teamwork"></a>Trabalho em equipe
- [Inscreva-se para alterar notificações no recurso de chat](teams-changenotifications-chat.md).
- [Inscreva-se para alterar notificações de usuários em um chat](teams-changenotifications-chatmembership.md), em um [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) ou em uma [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) (ou seja, recursos de [conversationMember](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true)).
- Obtenha detalhes de um evento que aconteceu em um chat, canal ou equipe, acessando [eventMessageDetail](/graph/api/resources/EventMessageDetail?view=graph-rest-beta&preserve-view=true) de um [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) ou [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true). Por exemplo, membros adicionados a um canal ou chat, e a descrição da equipe atualizada.


## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote nos novos recursos na [Comunidade Microsoft Tech](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de **_visualização_**. Todas as atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de **_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/office/dev-program), ganhe uma assinatura gratuita do Microsoft 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](https://developer.microsoft.com/graph/changelog/).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).
