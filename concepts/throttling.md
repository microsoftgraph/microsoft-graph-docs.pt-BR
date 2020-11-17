---
title: Diretrizes de limitação do Microsoft Graph
description: Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 56cd4925f7678e22b94eb97d4420b4a18c682ef7
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2020
ms.locfileid: "49030239"
---
# <a name="microsoft-graph-throttling-guidance"></a>Diretrizes de limitação do Microsoft Graph

Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.

Os limites de controle variam de acordo com o cenário. Por exemplo, se você estiver executando um grande volume de gravações, a possibilidade de limitação é mais alta do que se você estiver realizando apenas leituras.

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a>O que acontece quando a limitação ocorre?
<!-- markdownlint-enable MD026 -->

Quando um limite de controle é excedido, o Microsoft Graph limitas quaisquer outras solicitações desse cliente por um período. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (solicitações demais) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha. O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitação são limitados. Os limites de controle variam com base no tipo de solicitação. Portanto, você pode encontrar um cenário onde as gravações são limitadas, mas leituras ainda são permitidas.

## <a name="common-throttling-scenarios"></a>Cenários comuns de limitação

As causas mais comuns de limitação dos clientes incluem:

- Um grande número de solicitações em todos os aplicativos em um locatário.
- Um grande número de solicitações de um aplicativo específico entre todos os locatários.

## <a name="sample-response"></a>Resposta de amostra

Sempre que o limite de estrangulamento é excedido, o Microsoft Graph responde com uma resposta semelhante a esta.

```http
HTTP/1.1 429 Too Many Requests
Content-Type: application/json
Retry-After: 2.128

{
  "error": {
    "code": "TooManyRequests",
    "innerError": {
      "code": "429",
      "date": "2020-08-18T12:51:51",
      "message": "Please retry after",
      "request-id": "94fb3b52-452a-4535-a601-69e0a90e3aa2",
      "status": "429"
    },
    "message": "Please retry again later."
  }
}
```

## <a name="best-practices-to-handle-throttling"></a>Práticas recomendadas para lidar com a limitação

Estas são as práticas recomendadas para lidar com a limitação:

- Reduza o número de operações por solicitação.
- Reduza a frequência de chamadas.
- Evite novas tentativas imediatas, pois todas as solicitações se acumulam em relação aos seus limites de uso.

Quando você implementa a manipulação de erro, use o código de erro HTTP 429 para detectar a limitação. A resposta com falha inclui o campo `Retry-After` no cabeçalho de resposta. Desativar solicitações usando o atraso `Retry-After` é a forma mais rápida de se recuperar da limitação, já que o Microsoft Graph continua a registrar a utilização de recursos enquanto o cliente continua limitado.

1. Aguarde o número de segundos especificado no cabeçalho `Retry-After`.
2. Repita a solicitação.
3. Se a solicitação falhar novamente com um código de erro 429, você ainda estará limitado. Continue a usar o atraso `Retry-After` recomendado e repita a solicitação até obter êxito.

Todos os recursos e as APIs descritos na seção [limites específicos do serviço](#service-specific-limits) fornecem um `Retry-After`cabeçalho, exceto sob ressalva.

Para uma discussão mais ampla sobre a limitação no Microsoft Cloud, veja [Padrão de Limitação](/azure/architecture/patterns/throttling).

> [!NOTE]
> If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy. You can also implement [more advanced patterns](/azure/architecture/patterns/category/resiliency) when building large-scale applications.
>
> Os SDKs do Microsoft Graph já implementam manipuladores que dependem do cabeçalho `Retry-After` ou padrão para uma política de repetição de retirada exponencial.

## <a name="best-practices-to-avoid-throttling"></a>Práticas recomendadas para evitar a limitação

Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances. You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.

>[!NOTE]
>[Práticas recomendadas para descobrir arquivos e detectar alterações em escala](/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) descrevem as práticas recomendadas em detalhes.

## <a name="throttling-and-batching"></a>Limitação e dosagem

[JSON batching](./json-batching.md) allows you to optimize your application by combining multiple requests into a single JSON object. Requests in a batch are evaluated individually against throttling limits and if any request exceeds the limits, it fails with a `status` of `429` and an error similar to the one provided above. The batch itself fails with a status code of `424` (Failed Dependency). It is possible for multiple requests to be throttled in a single batch. You should retry each failed request from the batch using the value provided in the `retry-after` response header from the JSON content. You may retry all the failed requests in a new batch after the longest `retry-after` value.

Se os SDKs tentarem novamente as solicitações limitadas automaticamente quando não estiverem em lote, as solicitações limitadas que fizeram parte de um lote não serão automaticamente repetidas.

## <a name="service-specific-limits"></a>Limites específicos do serviço

Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory. These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.

Any request can be evaluated against multiple limits, depending on the scope of the limit (per app across all tenants, per tenant for all apps, per app per tenant, and so on), the request type (GET, POST, PATCH, and so on), and other factors. The first limit to be reached triggers throttling behavior. In addition to the service specific-limits described in the section, the following global limits apply:

| Tipo de solicitação | Por aplicativo em todos os locatários  |
| ------------ | ------------------------ |
| Qualquer          | 2000 solicitações por segundo |

> [!NOTE]
> Os limites específicos descritos aqui estão sujeitos a alterações.

> **Note:** In this section, the term *tenant* refers to the Microsoft 365 organization where the application is installed. This tenant can be the same as the the one where the application was created, in the case of a single tenant application, or it can be different, in the case of a [multi-tenant application](/azure/active-directory/develop/setup-multi-tenant-app).

### <a name="outlook-service-limits"></a>Limites de serviço do Outlook

Outlook service limits are evaluated for each app ID and mailbox combination. In other words, the limits described apply to a specific app accessing a specific mailbox (user or group). If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox. The following limits apply to the public cloud as well as [national cloud deployments](./deployments.md).

| Limite                                                      | Aplicável a      |
|------------------------------------------------------------|-----------------|
| 10.000 solicitações de API em um período de 10 minutos                  | pontos de extremidade v1.0 e beta |
| 4 solicitações simultâneas                                      | v1.0 e pontos finais beta   |
| 15 megabytes (MB) de upload (PATCH, POST, PUT) em um período de 30 segundos | v1.0 e pontos finais beta   |

#### <a name="outlook-service-resources"></a>Recursos de serviço do Outlook

Os recursos a seguir são fornecidos pelo serviço do Outlook.

##### <a name="search-api-resources-preview"></a>Pesquisar recursos da API (visualização)

- [Item externo (Pesquisa da Microsoft)](/graph/api/resources/externalitem?view=graph-rest-beta)

##### <a name="profile-api-resources"></a>Recursos da API de perfil

- [Foto](/graph/api/resources/profilephoto?view=graph-rest-1.0)

##### <a name="calendar-api-resources"></a>Recursos da API do calendário

- [event](/graph/api/resources/event)
- [eventMessage](/graph/api/resources/eventmessage)
- [calendar](/graph/api/resources/calendar)
- [calendarGroup](/graph/api/resources/calendargroup)
- [outlookCategory](/graph/api/resources/outlookcategory)
- [attachment](/graph/api/resources/attachment)
- [place (preview)](/graph/api/resources/place)

##### <a name="mail-api-resources"></a>Recursos da API do email

- [message](/graph/api/resources/message)
- [mailFolder](/graph/api/resources/mailfolder)
- [mailSearchFolder](/graph/api/resources/mailsearchfolder)
- [messageRule](/graph/api/resources/messagerule)
- [outlookCategory](/graph/api/resources/outlookcategory)
- [attachment](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a>Recursos da API de contatos pessoais

- [contato](/graph/api/resources/contact)
- [contactFolder](/graph/api/resources/contactfolder)
- [outlookCategory](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a>Recursos da inteligência social e do local de trabalho 

- [person](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a>Recursos da API de tarefas pendentes (visualização)

- [outlookTask](/graph/api/resources/outlooktask)
- [outlookTaskFolder](/graph/api/resources/outlooktaskfolder)
- [outlookTaskGroup](/graph/api/resources/outlooktaskgroup)
- [outlookCategory](/graph/api/resources/outlookcategory)
- [attachment](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a>Limites dos serviços de comunicação em nuvem

| Recurso      | Limites por aplicativo e por inquilino    |
| -------------- | ------------ |
| [Chamadas](/graph/api/resources/call) | 10.000 chamadas/mês e 100 chamadas simultâneas   |
| [Informações sobre a reunião ](/graph/api/resources/meetinginfo)   | 2000 reuniões/usuário a cada mês |
| [Presença](/graph/api/resources/presence) (pré-visualização)   | 50 solicitações por segundo |

### <a name="onenote-service-limits"></a>Limites do serviço OneNote

| Tipo de limite | Limitar por aplicativo por usuário (contexto delegado) | Limite por aplicativo (contexto somente de aplicativo) |
| ------------ | ------- | ------- |
| Taxa de solicitações | 120 solicitações por 1 minuto e 400 por 1 hora | 240 solicitações por 1 minuto e 800 por 1 hora |
| Solicitações simultâneas | 5 solicitações simultâneas | 20 solicitações simultâneas |

Os limites anteriores se aplicam aos seguintes recursos:  
onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation

Você pode encontrar informações adicionais sobre as práticas recomendadas no [limitação da API do OneNote e como evitá-la](https://developer.microsoft.com/pt-BR/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).  

> **Observação:** os recursos listados acima não retornam um cabeçalho `Retry-After` em respostas `429 Too Many Requests`.

### <a name="project-rome-service-limits"></a>Limites de serviços do Project Rome

| Tipo de solicitação | Limitar por usuário a todos os aplicativos |
| ------------ | --------------------------- |
| OBTER          | 400 solicitações a cada 5 minutos e 12000 solicitações por dia |
| POSTAR, COLOCAR, CORRIGIR, EXCLUIR | 100 solicitações a cada 5 minutos e 8000 solicitações por dia |

Os limites anteriores se aplicam aos seguintes recursos:  
activityHistoryItem, userActivity

### <a name="microsoft-teams-service-limits"></a>Limites do serviço do Microsoft Teams

Os limites são expressos como solicitações por segundo (rps).

| Tipo de solicitação do Teams                                   | Limitar por aplicativo por locatário        | Limitar por aplicativo em todos os locatários      |
|------------------------------------------------------|---------------------------------|------------|
| Todas as chamadas de API do Graph para o Microsoft Teams              | 15000 solicitações a cada 10 segundos | n/d |
| OBTER equipe, canal, guia, installedApps, appCatalogs   | 60 rps                          | 600 rps |
| Canal POST/PUT, guia, installedApps, appCatalogs    |  30 rps                         | 300 rps  |
| PATCH da equipe, canal, guia, installedApps, appCatalogs |  30 rps                         | 300 rps  |
| EXCLUIR canal, Tab, installedApps, appCatalogs      |  15 rps                         | 150 rps  |
| OBTER /teams/```{team-id}```, joinedTeams              |  30 rps                         | 300 rps  |
| POSTAR /teams/```{team-id}```, COLOCAR /groups/```{team-id}```/team, clone | 6 rps | 150 rps  |
| OBTER mensagem do canal  | 5 rps | 100 rps |
| OBTER 1:1/mensagem de chat do grupo  | 3 rps | 30 rps |
| POSTAR mensagem do canal | 2 rps | 20 rps |
| POSTAR 1:1/mensagem de chat do grupo | 2 rps | 20 rps |
| OBTENHA /equipes/```{team-id}```/programação e todas as APIs neste caminho | 60 rps | 600 rps |
| PUBLIQUE, CORRIJA, COLOQUE /equipes/```{team-id}```/ programação e todas as APIs neste caminho | 30 rps | 300 rps |
| APAGAR /equipe/```{team-id}```/programação e todas as APIs neste caminho | 15 rps | 150 rps |

A maximum of 4 requests per second per app can be issued on a given team or channel. A maximum of 3000 messages per app per day can be sent to a given channel.

Confira também [limites do Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) e [requisitos de votação](/graph/api/resources/teams-api-overview#polling-requirements).

Os limites anteriores se aplicam aos seguintes recursos:  
aadUserConversationMember, appCatalogs, changeTrackedEntity, channel, chatMessage, chatMessageHostedContent, conversationMember, offerShiftRequest, openShift, openShiftChangeRequest, schedule, scheduleChangeRequest, schedulingGroup, shift, shiftPreferences, swapShiftsChangeRequest, team, teamsApp, teamsAppDefinition, teamsAppInstallation, teamsAsyncOperation, teamsTab, teamsTemplate, teamwork, timeOff, timeOffReason, timeOffRequest, userSettings, workforceIntegration.

### <a name="identity-and-access-service-limits"></a>Limites do serviço de identidade e acesso

Estes limites de serviço se aplicam às seguintes entidades:

- [Objeto de diretório](/graph/api/resources/directoryobject)
- [Propriedade de extensão](/graph/api/resources/extensionproperty)
- [Unidade administrativa](/graph/api/resources/administrativeunit)
- [Aplicação](/graph/api/resources/application)
- [Atribuição de função da aplicação](/graph/api/resources/approleassignment)
- [Configuração de autentificação baseada em certificados](/graph/api/resources/certificatebasedauthconfiguration)
- [Contatos organizacionais](/graph/api/resources/orgcontact)
- [Dispositivo](/graph/api/resources/device)
- [Referência sobre o objetivo do parceiro do diretório](/graph/api/resources/directoryobjectpartnerreference)
- [Função de diretório](/graph/api/resources/directoryrole)
- [Modelo de função de diretório](/graph/api/resources/directoryroletemplate)
- [Domínio](/graph/api/resources/domain)
- [Registro dns domínio](/graph/api/resources/domaindnsrecord)
- [registro nome dns domínio](/graph/api/resources/domaindnscnamerecord)
- [Registro ms dns domínio](/graph/api/resources/domaindnsmxrecord)
- [Registro srv dns domínio](/graph/api/resources/domaindnssrvrecord)
- [Registro txt dns domínio](/graph/api/resources/domaindnstxtrecord)
- [Registro indisponível dns domínio](/graph/api/resources/domaindnsunavailablerecord)
- [Ponto de extremidade](/graph/api/resources/endpoint)
- [Propriedade de extensão](/graph/api/resources/extensionproperty)
- [Detalhes da licença](/graph/api/resources/licensedetails)
- [Grupo](/graph/api/resources/group)
- [Política de tempo limite baseada na atividade](/graph/api/resources/activitybasedtimeoutpolicy)
- [Política de mapeamento de declarações](/graph/api/resources/claimsmappingpolicy)
- [Política de descoberta de realm inicial](/graph/api/resources/homerealmdiscoverypolicy)
- [Política de emissão de tokens](/graph/api/resources/tokenissuancepolicy)
- [Política do tempo de vida do token](/graph/api/resources/tokenlifetimepolicy)
- [Base da política](/graph/api/resources/policybase)
- [Política de STS](/graph/api/resources/stspolicy)
- [Contrato](/graph/api/resources/contract)
- [Entidade de serviço](/graph/api/resources/serviceprincipal)
- [Sku inscrita](/graph/api/resources/subscribedsku)
- [Concessão de permissão do OAuth2](/graph/api/resources/oauth2permissiongrant)
- [Organização](/graph/api/resources/organization)
- [Usuário](/graph/api/resources/user)
- [Configuração de grupo](/graph/api/resources/groupsetting)
- [Modelo de configuração de grupo](/graph/api/resources/groupsettingtemplate)

#### <a name="pattern"></a>Padrão

Throttling is based on a token bucket algorithm, which works by adding individual costs of requests. The sum of request costs is then compared against pre-determined limits. Only the requests exceeding the limits will be throttled. If any of the limits are exceeded, the response will be `429 Too Many Requests`. It is possible to receive `429 Too Many Requests` responses even when the following limits are not reached, in situations when the services are under an important load or based on data volume for a specific tenant. The following table lists existing limits.

| Tipo de limite | Cota de unidade de recurso | Gravar cota |
| ---------- | ----------- | -------------- |
| aplicação+par de locatários | S: 3500, M:5000, L:8000 por 10 segundos | 3000 por 2 minutos e 30 segundos |
| aplicação | 150,000 por 20 segundos  | 70,000 por 5 minutos |
| locatário | Não Aplicável | 18,000 por 5 minutos |

> **Observação**: o limite do par aplicativo + locatário varia com base no número de usuários nas solicitações de locatário que são executadas. Os tamanhos dos locatários são definidos da seguinte forma: S - menos de 50 usuários, M - entre 50 e 500 usuários e L - acima de 500 usuários.

The following table lists base request costs. Any requests not listed have a base cost of 1.

| Operação | Caminho da Solicitação | Base do Custo Unitário de Recurso | Gravar Custo |
| --------- | ------------ | ----------------- | ------------------ |
| OBTER | `applications` | 2 | 0 |
| OBTER | `applications/{id}/extensionProperties` | 2 | 0 |
| OBTER | `contracts` | 3 | 0 |
| POSTAR | `directoryObjects/getByIds` |  3 | 0 |
| OBTER | `domains/{id}/domainNameReferences` | 4 | 0 |
| POSTAR | `getObjectsById` | 3 | 0 |
| OBTER | `groups/{id}/members` | 3 | 0 |
| OBTER | `groups/{id}/transitiveMembers` | 5 | 0 |
| POSTAR | `isMemberOf` | 4 | 0 |
| POSTAR | `me/checkMemberGroups` | 4 | 0 |
| POSTAR | `me/checkMemberObjects` | 4 | 0 |
| POSTAR | `me/getMemberGroups` | 2 | 0 |
| POSTAR | `me/getMemberObjects` | 2 | 0 |
| OBTER | `me/licenseDetails` | 2 | 0 |
| OBTER | `me/memberOf` | 2 | 0 |
| OBTER | `me/ownedObjects` | 2 | 0 |
| OBTER | `me/transitiveMemberOf` | 2 | 0 |
| OBTER | `oauth2PermissionGrants` | 2 | 0 |
| OBTER | `oauth2PermissionGrants/{id}` | 2 | 0 |
| OBTER | `servicePrincipals/{id}/appRoleAssignments` | 2 | 0 |
| OBTER | `subscribedSkus` | 3 | 0 |
| OBTER | `users` | 2 | 0 |
| OBTER | Qualquer caminho de identidade não listado na tabela | 1 | 0 |
| POSTAR | Qualquer caminho de identidade não listado na tabela | 1 | 1 |
| PATCH | Qualquer caminho de identidade não listado na tabela | 1 | 1 |
| PUT | Qualquer caminho de identidade não listado na tabela | 1 | 1 |
| EXCLUIR | Qualquer caminho de identidade não listado na tabela | 1 | 1 |

Outros fatores que afetam um custo da solicitação:

- Usar o `$select` reduz os custos por 1
- Usar o `$expand` aumenta os custos por 1
- Usar o `$top` com um valor menor que 20 reduz os custos por 1

> **Note:** A request cost can never be lower than 1. Any request cost that applies to a request path starting with `me/` also applies to equivalent requests starting with `users/{id | userPrincipalName}/`.

#### <a name="additional-headers"></a>Cabeçalhos adicionais

##### <a name="request-headers"></a>Cabeçalhos de solicitação

- **x-ms-throttle-priority** - If the header doesn't exist or is set to any other value, it indicates a normal request. We recommend setting priority to `high` only for the requests initiated by the user. The values of this header can be the following:
  - Low - Indicates the request is low priority. Throttling this request doesn't cause user-visible failures.
  - Normal - Default if no value is provided. Indicates that the request is default priority.
  - High - Indicates that the request is high priority. Throttling this request causes user-visible failures.

> **Note:** Should requests be throttled, low priority requests will be throttled first, normal priority requests second, and high priority requests last. Using the priority request header does not change the limits.

##### <a name="regular-responses-requests"></a>Solicitações de respostas regulares

- **x-ms-resource-unit** - Indicates the resource unit used for this request. Values are positive integers.
- **x-ms-throttle-limit-percentage** - Returned only when the application consumed more than 0.8 of its limit. The value ranges from 0.8 to 1.8 and is a percentage of the use of the limit. The value can be used by the callers to set up an alert and take action.

##### <a name="throttled-responses-requests"></a>Solicitações de respostas limitadas

- **x-ms-throttle-scope** - eg. `Tenant_Application/ReadWrite/9a3d526c-b3c1-4479-ba74-197b5c5751ae/0785ef7c-2d7a-4542-b048-95bcab406e0b`. Indicates the scope of throttling with the following format `<Scope>/<Limit>/<ApplicationId>/<TenantId|UserId|ResourceId>`:
  - Escopo: (cadeia de caracteres, obrigatório)
    - Tenant_Application - Todas as solicitações para um determinado locatário da aplicação atual.
    - Tenant - Todas as solicitações para o locatário atual, independentemente da aplicação.
    - Application - Todas solicitações para a aplicação atual.
  - Limit: (cadeia de caracteres, obrigatório)
    - Read: Solicitações de leitura do escopo (GET)
    - Write: Solicitações de gravação do escopo (POST, PATCH, PUT, DELETE...)
    - ReadWrite: Todas solicitações do escopo (qualquer)
  - ApplicationId (GUID, obrigatório)
  - TenantId|UserId|ResourceId: (GUID, obrigatório)
- **x-ms-throttle-information** - Indicates the reason for throttling and can have any value (string). The value is provided for diagnostics and troubleshooting purposes, some examples include:
  - CPULimitExceeded - Limitando porque o limite para alocação do CPU está excedido.
  - WriteLimitExceeded - limitando porque o limite para gravação está excedido.
  - ResourceUnitLimitExceeded - Limitando porque o limite para a unidade de recurso alocada foi excedido.

### <a name="information-protection"></a>Proteção de informações

Os seguintes limites se aplicam a qualquer solicitação no `/informationProtection`.

| Operation                 | Limite por inquilino                                            | Limite por recurso (email, URL, arquivo)                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| POST                      | 150 solicitações a cada 15 minutos e 10000 solicitações a cada 24 horas | 1 solicitação a cada 15 minutos e 3 solicitações a cada 24 horas |

Os limites anteriores se aplicam aos seguintes recursos:  
threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.

### <a name="identity-protection-and-conditional-access-service-limits"></a>Proteção da identidade e limites do serviço de acesso condicional

| Tipo de solicitação | Limitar por locatário para todos os aplicativos |
| ------------ | ------- |
| Qualquer | 1 solicitação por segundo |

Os limites anteriores aplicam-se aos seguintes recursos:  
Detecçãoderisco, Usuárioderisco, HistóricodeItemdeUsuárioderisco, NomedoLocal, paísNomedoLocal, ipNomedoLocal, PolíticadeAcessoCondicional.

> **Observação:** os recursos listados acima não retornam um cabeçalho `Retry-After` em respostas `429 Too Many Requests`.

### <a name="insights-service-limits"></a>Percepção dos limites de serviço

Os seguintes limites se aplicam a qualquer pedido em `me/insights` ou `users/{id}/insights`.

| Limite                                                      | Aplicável a      |
|------------------------------------------------------------|-----------------|
| 10.000 solicitações de API em um período de 10 minutos                  | pontos de extremidade v1.0 e beta |
| 4 solicitações simultâneas                                      | v1.0 e pontos finais beta   |

Os limites anteriores se aplicam aos seguintes recursos:  
pessoas, tendências, usedinsight, sharedInsight.

### <a name="microsoft-graph-reports-service-limits"></a>Limites do serviço de relatórios do Microsoft Graph

Os seguintes limites se aplicam a qualquer solicitação no `/reports`.

| Operation                 | Limitar por aplicativo por locatário     | Limitar por locatário para todos os aplicativos |
|---------------------------|------------------------------|----------------------------|
| Qualquer pedido (CSV)         | 14 solicitações a cada 10 minutos   | 40 solicitações a cada 10 minutos |
| Qualquer solicitação (JSON, beta)  | 100 solicitações a cada 10 minutos  | n/d                        |

The preceding limits apply individually to each report API. For example, a request to the Microsoft Teams user activity report API and a request to the Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.

Os limites anteriores se aplicam aos seguintes recursos de **relatório**.  

### <a name="invitation-manager-service-limits"></a>Limites de serviço do gerenciador de convite

Os seguintes limites se aplicam a qualquer solicitação no `/invitations`.

| Operation                 | Limitar por locatário para todos os aplicativos |
|---------------------------|------------------------------|
| Qualquer operação             | 150 solicitações a cada 5 segundos   |

### <a name="security-detections-and-incidents-service-limits"></a>Limites de serviços de detecção de segurança e incidentes

Os seguintes limites se aplicam a qualquer solicitação no `/security`.

| Operation                  | Limitar por aplicativo por locatário     |
|----------------------------|------------------------------|
| Qualquer operação em `alert`, `securityActions`,  `secureScore` | 150 solicitações por minuto      |
| Qualquer operação em `tiIndicator` | 1000 solicitações por minuto |
| Qualquer operação em `secureScore` ou `secureScorecontrolProfile` | 10.000 solicitações de API em um período de 10 minutos |
| Qualquer operação em `secureScore` ou `secureScorecontrolProfile` | 4 solicitações simultâneas |

### <a name="open-and-schema-extensions-service-limits"></a>Limitações de serviços à extensões de esquema e abertas

| Tipo de solicitação | Limitar por aplicativo por locatário |
| ------------ | ------------------------ |
| Qualquer          | 455 solicitações a cada 10 segundos |

Os limites acima se aplicam aos seguintes recursos: openTypeExtension, schemaExtension, administrativeUnit, contato, dispositivo, evento, grupo, mensagem, organização, postagem e usuário.

### <a name="files-and-lists-service-limits"></a>Limites de serviço dos arquivos e listas

Service limits for OneDrive, OneDrive for Business, and SharePoint Online are not available. For more information, see [why can't you just tell me the exact throttling limits?](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits).

As informações anteriores aplicam-se aos seguintes recursos:  
baseItem, baseItemVersion, columnDefinition, columnLink, contentType, drive, driveItem, driveItemVersion, fieldValueSet, itemActivity, itemActivityStat, List, listItem, listItemVersion, permission, sharedDriveItem, site e thumbnailSet.

### <a name="tasks-and-plans-service-limits"></a>Limites de serviços de tarefas e planos

Os limites de serviço do Planner não estão disponíveis.

As informações anteriores aplicam-se aos seguintes recursos:  
planner, plannerAssignedToTaskBoardTaskFormat, plannerBucket, plannerBucketTaskBoardTaskFormat, plannerGroup, plannerPlan, plannerPlanDetails, plannerProgressTaskBoardTaskFormat, plannerTask, plannerTaskDetails, e plannerUser.

### <a name="identity-and-access-data-policy-operation-service-limits"></a>Limites de operação de serviços de política de dados de identidade e acesso

| Tipo de solicitação | Limite por inquilino |
| ------------ | ---------------- |
| Postar no `exportPersonalData` | 1.000 solicitações por dia para todos os assuntos e 100 por assunto por dia |
| Qualquer outra solicitação | 10.000 solicitações por minuto |

Os limites anteriores se aplicam aos seguintes recursos: dataPolicyOperation.

> **Observação:** os recursos listados acima não retornam um cabeçalho `Retry-After` nas respostas `429 Too Many Requests`.

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a>Limites do serviço de Educação

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a>Limites de serviço do Excel

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a>Limites do serviço de registros de auditoria de identidade e acesso

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a>Limites de serviço dos fornecedores de identidade

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a>Limites de serviço Intune

[!INCLUDE [Intune applications throttling documentation](../includes/throttling-intune-applications.md)]
[!INCLUDE [Intune books throttling documentation](../includes/throttling-intune-books.md)]
[!INCLUDE [Intune company terms throttling documentation](../includes/throttling-intune-company-terms.md)]
[!INCLUDE [Intune device configuration throttling documentation](../includes/throttling-intune-device-configuration.md)]
[!INCLUDE [Intune device enrollment throttling documentation](../includes/throttling-intune-device-enrollment.md)]
[!INCLUDE [Intune devices throttling documentation](../includes/throttling-intune-devices.md)]
[!INCLUDE [Intune enrollment throttling documentation](../includes/throttling-intune-enrollment.md)]
[!INCLUDE [Intune managed applications throttling documentation](../includes/throttling-intune-managed-applications.md)]
[!INCLUDE [Intune notifications throttling documentation](../includes/throttling-intune-notifications.md)]
[!INCLUDE [Intune rbac throttling documentation](../includes/throttling-intune-rbac.md)]
[!INCLUDE [Intune remote assistance throttling documentation](../includes/throttling-intune-remote-assistance.md)]
[!INCLUDE [Intune reporting throttling documentation](../includes/throttling-intune-reporting.md)]
[!INCLUDE [Intune TEM throttling documentation](../includes/throttling-intune-tem.md)]
[!INCLUDE [Intune troubleshooting throttling documentation](../includes/throttling-intune-troubleshooting.md)]
[!INCLUDE [Intune wip throttling documentation](../includes/throttling-intune-wip.md)]

### <a name="skype-service-limits"></a>Limites do serviço Skype

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a>Limites do serviço de assinatura

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
