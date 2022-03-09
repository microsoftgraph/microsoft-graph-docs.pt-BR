---
title: Trabalhar com APIs de comunicações de serviço na Microsoft Graph
description: Você pode usar a API de comunicações de serviço na Microsoft Graph acessar o status de saúde e as postagens do centro de mensagens sobre serviços Microsoft".
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 6dd9abc0b3bd8bf71f46739df06a1b8c609fe2be
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367900"
---
# <a name="working-with-service-communications-api-in-microsoft-graph"></a>Trabalhar com a API de comunicações de serviço no Microsoft Graph
A API de comunicações de serviço fornece postagens de centro de mensagens e de saúde do serviço pertencentes aos serviços de nuvem da Microsoft inscritos pelo locatário. Você pode obter dados de saúde atuais e históricos de um serviço microsoft (por exemplo, o serviço Exchange Online está para baixo). Você pode verificar a saúde do serviço para determinar se um problema foi rastreado e uma resolução está em andamento antes de chamar o suporte ou passar o tempo solucionando problemas. As postagens da central de mensagens permitem que você acompanhe as próximas alterações, incluindo novos recursos, atualizações e outros comunicados importantes (por exemplo, Exchange Online está recebendo um novo recurso).

## <a name="authorization"></a>Autorização
O Microsoft Graph permite que os aplicativos tenham acesso autorizado à saúde e alterem comunicações sobre um serviço de nuvem da Microsoft inscrito por um locatário. Com as permissões delegadas ou de aplicativo [apropriadas](/graph/permissions-reference#service-communications-permissions), seu aplicativo pode acessar os dados de comunicações em nome de um usuário inscrevado ou sem qualquer usuário de entrada no locatário. Os tipos delegados e de aplicativos dessas permissões são concedidos apenas por um administrador.

Para obter mais informações sobre tokens de acesso, registro de aplicativo e permissões delegadas e de aplicativos, consulte [Noções básicas de autenticação e autorização](/graph/auth/auth-concepts).

### <a name="access-service-communications-api-on-behalf-of-signed-in-user"></a>API de comunicações de serviço de acesso em nome do usuário interno

As permissões delegadas são necessárias para acessar a API de comunicações de serviço em nome de um usuário interno. Aplicativos de tela voltados para o cliente, como o Centro de administração do Microsoft 365 (acessível apenas a funções de administrador), podem chamar [a](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/homepage) API de comunicações de serviço para obter os dados de comunicados de serviço e de serviço para o locatário do usuário in-locatário _, em_ nome do usuário in-locatário. Os usuários podem descobrir se seus serviços inscritos são saudáveis ou têm problemas. Eles também podem aprender sobre quaisquer problemas de serviço atuais que afetam seus locatários. 

### <a name="access-service-communications-api-without-user"></a>Api de comunicações de serviço de acesso sem usuário

As permissões de aplicativo são necessárias para acessar a API de comunicações de serviço sem um usuário interno. Aplicativos que são executados como serviços de back-end, como serviços de monitoramento ou alerta, podem chamar a API de comunicações de serviço com sua própria identidade e não em nome de um usuário. Esses serviços back-end podem criar pipelines de monitoramento/alerta personalizados e chamar a API de comunicações de serviço para obter dados de comunicados de serviço e integridade do serviço. 


## <a name="common-use-cases-and-required-permissions"></a>Casos de uso comum e permissões necessárias

|Casos de uso|Solicitações de API| Permissões obrigatórias| Tipos de permissão com suporte|
|:--------|:--------|:--------|:--------|
| Listar visão geral de saúde para locatário | [Listar healthOverviews](/graph/api/serviceannouncement-list-healthoverviews?view=graph-rest-beta&preserve-view=true) | _ServiceHealth.Read.All_ | Delegado e aplicativo | 
| Obter informações específicas de saúde do serviço para locatário | [Obter serviceHealth](/graph/api/servicehealth-get?view=graph-rest-beta&preserve-view=true) | _ServiceHealth.Read.All_ | Delegado e aplicativo |
| Listar todos os problemas de serviço para locatário | [Listar problemas](/graph/api/serviceannouncement-list-issues?view=graph-rest-beta&preserve-view=true) | _ServiceHealth.Read.All_ | Delegado e aplicativo |
| Obter um problema de serviço específico para locatário | [Obter problema](/graph/api/servicehealthissue-get?view=graph-rest-beta&preserve-view=true) | _ServiceHealth.Read.All_ | Delegado e aplicativo |
| Obter um relatório de revisão pós-incidente para locatário | [Obter relatório de incidentes](/graph/api/servicehealthissue-incidentreport?view=graph-rest-beta&preserve-view=true)| _ServiceHealth.Read.All_ | Delegado e aplicativo |
| Listar todas as mensagens de serviço para locatário | [Listar mensagens](/graph/api/serviceannouncement-list-messages?view=graph-rest-beta&preserve-view=true) | _ServiceMessage.Read.All_ | Delegado e aplicativo |
| Obter uma mensagem de serviço específica para locatário | [Obter mensagem](/graph/api/serviceupdatemessage-get?view=graph-rest-beta&preserve-view=true) | _ServiceMessage.Read.All_ | Delegado e aplicativo |
| Atualizar o status da mensagem de serviço para o usuário que está assinado | Para uma lista de operações de status, consulte [serviceUpdateMessage](/graph/api/resources/serviceupdatemessage?view=graph-rest-beta&preserve-view=true).| _ServiceMessageViewpoint.Write_ | Delegado |

## <a name="availability-in-national-clouds"></a>Disponibilidade em nuvens nacionais
Essa API de comunicações de serviço está disponível em todas as implantações de nuvem nacionais da Microsoft. Você pode obter dados de comunicações e de saúde do serviço para todos os locatários nas nuvens nacionais da Microsoft. Para obter detalhes, consulte [implantações de nuvem nacionais](/graph/deployments).

|Nuvens nacionais|URL da API (parcial)|
|:--------------|:-----------------|
|Serviço global do Microsoft Graph| https://graph.microsoft.com/beta/admin/serviceAnnouncement/|
|Microsoft Graph para o Governo dos EUA L4 (GccHigh)|https://graph.microsoft.us/beta/admin/serviceAnnouncement/|
|Microsoft Graph para o Us Government L5 (DoD)|https://dod-graph.microsoft.us/beta/admin/serviceAnnouncement/|
|Microsoft Graph Alemanha|https://graph.microsoft.de/beta/admin/serviceAnnouncement/|
|Microsoft Graph China operado pela 21Vianet|https://microsoftgraph.chinacloudapi.cn/beta/admin/serviceAnnouncement/|

## <a name="service-communications-limits"></a>Limites de comunicações de serviço

Para garantir o desempenho do serviço, a API de comunicações de serviço tem limites de limitação para as solicitações por locatário por aplicativo. Para obter detalhes sobre os limites, consulte  [limites de limitação para o serviço de comunicações de serviço](/graph/throttling#service-communications-service-limits).


## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas

A API de comunicações de serviço pode abrir novas maneiras de você se envolver com os usuários:

- [Visão geral para acessar as comunicações e a integridade do serviço no Microsoft Graph](/graph/service-communications-concept-overview)
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/partners).
