---
title: Diretrizes de limitação do Microsoft Graph
description: Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 482b4cd4dba1c3cf7e2f726820480bd5e990df35
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151507"
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
> Se nenhum cabeçalho `Retry-After` for fornecido pela resposta, recomendamos implementar uma política de repetição exponencial de retirada. Você também pode implementar [padrões mais avançados](/azure/architecture/patterns/category/resiliency) ao criar aplicativos em grande escala.
>
> Os SDKs do Microsoft Graph já implementam manipuladores que dependem do cabeçalho `Retry-After` ou padrão para uma política de repetição de retirada exponencial.

## <a name="best-practices-to-avoid-throttling"></a>Práticas recomendadas para evitar a limitação

Padrões de programação como pesquisando continuamente um recurso para verificar se há atualizações e a verificação regular das coleções de recursos para verificar se há recursos novos ou excluídos, possuem maior propensão de levar aplicativos a serem regulados e prejudicam o desempenho geral. Em vez disso, você deve aproveitar o [controle de alterações](delta-query-overview.md) e [notificações de alteração](webhooks.md) quando estiverem disponíveis.

>[!NOTE]
>[Práticas recomendadas para descobrir arquivos e detectar alterações em escala](/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) descrevem as práticas recomendadas em detalhes.

## <a name="throttling-and-batching"></a>Limitação e dosagem

[O lote JSON](./json-batching.md) permite que você otimize seu aplicativo combinando várias solicitações em um único objeto JSON. As solicitações em um lote são avaliadas individualmente em relação aos limites de estrangulamento e, se alguma solicitação exceder os limites, ela falhará com um `status` de `429` e um erro semelhante ao fornecido acima. O próprio lote falha com um código de status de `424` (Dependência com Falha). É possível que várias solicitações sejam limitadas em um único lote. Você deve tentar novamente a cada solicitação com falha no lote utilizando o valor fornecido no cabeçalho de resposta `retry-after` do conteúdo JSON. Você pode tentar novamente para todas as solicitações com falha em um novo lote após o valor `retry-after` mais longo.

Se os SDKs tentarem novamente as solicitações limitadas automaticamente quando não estiverem em lote, as solicitações limitadas que fizeram parte de um lote não serão automaticamente repetidas.

## <a name="service-specific-limits"></a>Limites específicos do serviço

O Microsoft Graph permite que você acesse os dados em [vários serviços](overview-major-services.md), como o Outlook ou o Azure Active Directory. Esses serviços impõem seus próprios limites de controle que afetam os aplicativos que usam o Microsoft Graph para acessá-los.

Qualquer solicitação poderá ser avaliada em relação a vários limites, dependendo do escopo do limite (por aplicativo em todos os locatários, por locatário para todos os aplicativos, por aplicativo por locatário, e assim por diante), do tipo de solicitação (GET, POST, PATCH e assim por diante) e de outros fatores. O primeiro limite a ser alcançado dispara o comportamento de limitação. Além dos limites de serviço específicos descritos na seção, os seguintes limites globais se aplicam:

| Tipo de solicitação | Por aplicativo em todos os locatários  |
| ------------ | ------------------------ |
| Qualquer          | 2000 solicitações por segundo |

> [!NOTE]
> Os limites específicos descritos aqui estão sujeitos a alterações.

> **Nota:** Nesta seção, o termo *locatário* refere-se à organização Microsoft 365 onde o aplicativo está instalado. Este inquilino pode ser o mesmo onde o aplicativo foi criado, no caso de um único aplicativo de inquilino, ou pode ser diferente, no caso de [um aplicativo de vários inquilinos](/azure/active-directory/develop/setup-multi-tenant-app).

### <a name="outlook-service-limits"></a>Limites de serviço do Outlook

Os limites de serviço do Outlook são avaliados para cada combinação de ID de aplicativo e caixa de correio. Em outras palavras, os limites descritos se aplicam a um aplicativo específico ao acessar uma caixa de correio específica (usuário ou grupo). Se um aplicativo exceder o limite de uma caixa de correio, isso não afetará a capacidade de acessar outra caixa de correio. Os seguintes limites se aplicam à nuvem pública, bem como às [ implementações de nuvens nacionais](./deployments.md).

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
| [Presença](/graph/api/resources/presence) (pré-visualização)   | 1.500 solicitações em um período de 30 segundos, por aplicativo por locatário |

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

É possível emitir, no máximo, 4 solicitações por segundo por aplicativo em uma determinada equipe ou canal.
Um máximo 3.000 mensagens por aplicativo por dia podem ser enviadas para um determinado canal.

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

A limitação baseia-se em um algoritmo no bucket de token, que funciona adicionando custos individuais de solicitações. A soma dos custos da solicitação é depois comparada contra os limites predeterminados. Apenas as solicitações que excedem os limites serão limitadas. Se qualquer um dos limites for excedido, a resposta será `429 Too Many Requests`. É possível receber respostas `429 Too Many Requests` mesmo quando os seguintes limites não são alcançados, em situações em que os serviços estão sob uma carga importante ou com base no volume de dados para um determinado locatário. A tabela a seguir lista os limites existentes.

| Tipo de limite | Cota de unidade de recurso | Gravar cota |
| ---------- | ----------- | -------------- |
| aplicação+par de locatários | S: 3500, M:5000, L:8000 por 10 segundos | 3000 por 2 minutos e 30 segundos |
| aplicação | 150,000 por 20 segundos  | 70,000 por 5 minutos |
| locatário | Não aplicável | 18,000 por 5 minutos |

> **Observação**: A aplicação + limite do par de locatários varia dependendo do número de usuários nas solicitações de locatário. Os tamanhos dos locatários são definidos da seguinte maneira: S - em 50 usuários, M - entre 50 e 500 usuários, e L para acima de 500 usuários.

A tabela a seguir lista a base dos custos da solicitação. Qualquer solicitação não listada tem um custo base de 1.

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

> **Observação:** Um custo da solicitação nunca pode ser menor do que 1. Qualquer custo da solicitação que se aplica a um caminho da solicitação iniciado por `me/` também se aplica a solicitações equivalentes iniciadas por `users/{id | userPrincipalName}/`.

#### <a name="additional-headers"></a>Cabeçalhos adicionais

##### <a name="request-headers"></a>Cabeçalhos de solicitação

- **x-ms-throttle-priority** - se o cabeçalho não existir ou se estiver definido com qualquer outro valor, ele indicará uma solicitação normal. Recomendamos definir a prioridade para `high` somente para as solicitações iniciadas pelo usuário. Os valores desse cabeçalho podem ser os seguintes:
  - Baixa - Indica que a solicitação tem prioridade baixa. Limitando esta solicitação não causa falhas visíveis ao usuário.
  - Normal - Padrão se nenhum valor for fornecido. Indica que a solicitação é a de prioridade padrão.
  - Alta - Indica que a solicitação é de alta prioridade. Limitando esta solicitação causa falhas visíveis ao usuário.

> **Observação:** Se as solicitações forem limitadas, as solicitações de baixa prioridade serão limitadas primeiro, as solicitações de prioridade normal em segundo e as solicitações de alta prioridade por último. Usar a prioridade no cabeçalho da solicitação não altera os limites.

##### <a name="regular-responses-requests"></a>Solicitações de respostas regulares

- **x-ms-resource-unit** - Indica a unidade de recurso usada para esta solicitação. Os valores são números inteiros positivos.
- **x-ms-throttle-limit-percentage** - Retornado somente quando a aplicação consumiu mais de 0.8 de seu limite. O valor varia de 0.8 a 1.8 e é uma porcentagem do uso do limite. O valor pode ser usado pelos chamadores para configurar um alerta e tomar providências.

##### <a name="throttled-responses-requests"></a>Solicitações de respostas limitadas

- **x-ms-throttle-scope** - exemplo. `Tenant_Application/ReadWrite/9a3d526c-b3c1-4479-ba74-197b5c5751ae/0785ef7c-2d7a-4542-b048-95bcab406e0b`. Indica o escopo de limitação com o seguinte formato `<Scope>/<Limit>/<ApplicationId>/<TenantId|UserId|ResourceId>`:
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
- **x-ms-throttle-information** - Indica o motivo para a limitação e pode ter qualquer valor (cadeia de caracteres). O valor é fornecido para fins de solução de problemas e diagnósticos. Alguns exemplos incluem:
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

Os limites anteriores aplicam-se individualmente a cada relatório de API. Por exemplo, uma solicitação da API do relatório de atividades do usuário do Microsoft Teams e uma solicitação de relatório da API do usuário do Outlook dentro de 10 minutos contará como uma solicitação entre 14 para cada API e não duas solicitações entre 14 para ambas.

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

Os limites de serviço do OneDrive, OneDrive for Business e SharePoint Online não estão disponíveis. Para mais informações, confira [Por que não é possível saber o limites exatos?](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits).

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

### <a name="assignment-service-limits"></a>Limites de serviço de atribuição

Os limites a seguir se aplicam às solicitações na API do serviço de atribuição:

| Tipo de solicitação                 | Limitar por aplicativo por locatário     | Limitar por locatário para todos os aplicativos |
|---------------------------|------------------------------|----------------------------|
| Qualquer         | 5000 solicitações a cada 10 segundos   | 15.000 solicitações a cada 10 segundos |
| GET me/Assignment  | 50 solicitações a cada 10 segundos | 150 solicitações a cada 10 segundos |  

Os limites anteriores se aplicam aos seguintes recursos: [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest)
[educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest)
[educationResource](/graph/api/resources/educationresource?view=graph-rest)
