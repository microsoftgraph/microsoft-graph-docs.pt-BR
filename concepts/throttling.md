---
title: Diretrizes de limitação do Microsoft Graph
description: Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 6f37fdf90f510a650f2b1d13c42e83636c22697a
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133346"
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

Padrões de programação, como pesquisar continuamente um recurso para verificar atualizações e verificar regularmente coleções de recursos para verificar recursos novos ou excluídos, são mais propensos a fazer com que os aplicativos sejam limitados e degradem o desempenho geral. Em vez disso, você deve aproveitar [controle de alterações](delta-query-overview.md) e [notificações de alterações](webhooks.md) quando disponíveis.

>[!NOTE]
>[Práticas recomendadas para descobrir arquivos e detectar alterações em escala](/onedrive/developer/rest-api/concepts/scan-guidance) descrevem as práticas recomendadas em detalhes.

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

| API                                                      | Recursos      |
|------------------------------------------------------------|-----------------|
| Pesquisar API (visualização)                  | <li>[Item externo (Pesquisa da Microsoft)](/graph/api/resources/externalitem) |
| API de perfil                                      | <li>[Foto](/graph/api/resources/profilephoto)   |
| API de Calendário | <li>[event](/graph/api/resources/event) <li> [eventMessage](/graph/api/resources/eventmessage) <li> [calendar](/graph/api/resources/calendar) <li>  [calendarGroup](/graph/api/resources/calendargroup) <li> [outlookCategory](/graph/api/resources/outlookcategory) <li> [attachment](/graph/api/resources/attachment) <li> [place (preview)](/graph/api/resources/place)   |
| API de Email do Outolook                                      | <li>[message](/graph/api/resources/message) <li>  [message](/graph/api/resources/message) <li> [mailFolder](/graph/api/resources/mailfolder) <li> [mailSearchFolder](/graph/api/resources/mailsearchfolder) <li> [messageRule](/graph/api/resources/messagerule) <li> [outlookCategory](/graph/api/resources/outlookcategory) <li> [attachment](/graph/api/resources/attachment)|
| API de contatos pessoais | <li>[contato](/graph/api/resources/contact) <li> [contactFolder](/graph/api/resources/contactfolder) <li> [outlookCategory](/graph/api/resources/outlookcategory)|
| Inteligência social e do local de trabalho | <li>[pessoa](/graph/api/resources/person) |
| API de tarefas pendentes (visualização) | <li>[outlookTask](/graph/api/resources/outlooktask) <li> [outlookTaskFolder](/graph/api/resources/outlooktaskfolder) <li>[outlookTaskGroup](/graph/api/resources/outlooktaskgroup) <li> [outlookCategory](/graph/api/resources/outlookcategory) <li> [attachment](/graph/api/resources/attachment)|


### <a name="cloud-communication-service-limits"></a>Limites dos serviços de comunicação em nuvem

| Recurso      | Limites por aplicativo    |
| -------------- | ------------ |
| [Chamadas](/graph/api/resources/call) | 10.000 chamadas/mês e 100 chamadas simultâneas   |
| [Informações sobre a reunião ](/graph/api/resources/meetinginfo)   | 2000 reuniões/usuário a cada mês |
| [Presença](/graph/api/resources/presence)   | 1.500 solicitações em um período de 30 segundos, por aplicativo por locatário |

### <a name="onenote-service-limits"></a>Limites do serviço OneNote

| Tipo de limite | Limitar por aplicativo por usuário (contexto delegado) | Limite por aplicativo (contexto somente de aplicativo) |
| ------------ | ------- | ------- |
| Taxa de solicitações | 120 solicitações por 1 minuto e 400 por 1 hora | 240 solicitações por 1 minuto e 800 por 1 hora |
| Solicitações simultâneas | 5 solicitações simultâneas | 20 solicitações simultâneas |

Os limites anteriores se aplicam aos seguintes recursos:

[!INCLUDE [Onenote throttling documentation](../includes/throttling-onenote.md)]

Você pode encontrar informações adicionais sobre as práticas recomendadas no [limitação da API do OneNote e como evitá-la](https://developer.microsoft.com/en-us/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).

**Observação:** os recursos listados acima não retornam um cabeçalho `Retry-After` em respostas `429 Too Many Requests`.

### <a name="project-rome-service-limits"></a>Limites de serviços do Project Rome

| Tipo de solicitação | Limitar por usuário a todos os aplicativos |
| ------------ | --------------------------- |
| OBTER          | 400 solicitações a cada 5 minutos e 12000 solicitações por dia |
| POSTAR, COLOCAR, CORRIGIR, EXCLUIR | 100 solicitações a cada 5 minutos e 8000 solicitações por dia |

Os limites anteriores se aplicam aos seguintes recursos:

- [activityHistoryItem](/graph/api/resources/activityhistoryitem)
- [userActivity](/graph/api/resources/useractivity)

### <a name="microsoft-teams-service-limits"></a>Limites do serviço do Microsoft Teams

Os limites são expressos como solicitações por segundo (rps).

| Tipo de solicitação do Teams                                   | Limitar por aplicativo por locatário        | Limitar por aplicativo em todos os locatários      |
|------------------------------------------------------|---------------------------------|------------|
| OBTER equipe, canal, guia, installedApps, appCatalogs   | 30 rps                          | 600 rps |
| Canal POST/PUT, guia, installedApps, appCatalogs    |  30 rps                         | 300 rps  |
| PATCH da equipe, canal, guia, installedApps, appCatalogs |  30 rps                         | 300 rps  |
| EXCLUIR canal, Tab, installedApps, appCatalogs      |  15 rps                         | 150 rps  |
| OBTER /teams/```{team-id}```, joinedTeams              |  30 rps                         | 300 rps  |
| POST /equipes | 10 rps | 100 rps  |
| PUT /grupos/```{team-id}```/equipe, clonar | 6 rps | 150 rps  |
| OBTER mensagem do canal  | 20 rps | 200 rps |
| OBTER 1:1/mensagem de chat do grupo  | 20 rps | 200 rps |
| POSTAR mensagem do canal | 50 rps | 500 rps |
| POSTAR 1:1/mensagem de chat do grupo | 20 rps | 200 rps |
| OBTENHA /equipes/```{team-id}```/programação e todas as APIs neste caminho | 30 rps | 600 rps |
| PUBLIQUE, CORRIJA, COLOQUE /equipes/```{team-id}```/ programação e todas as APIs neste caminho | 30 rps | 300 rps |
| APAGAR /equipe/```{team-id}```/programação e todas as APIs neste caminho | 15 rps | 150 rps |
| POST /equipes/```{team-id}```/sendActivityNotification | 5 rps | 50 rps |
| POST /chats/```{chat-id}```/sendActivityNotification | 5 rps | 50 rps |
| POST /usuários/```{user-id}```/teamwork/sendActivityNotification | 5 rps | 50 rps |
| Outras chamadas à API GET para o Microsoft Teams              | 30 rps | 1500 rps |
| Outras chamadas à API para o Microsoft Teams              | 30 rps | 300 rps |

É possível emitir, no máximo, 4 solicitações por segundo por aplicativo em uma determinada equipe ou canal.
Um máximo 3.000 mensagens por aplicativo por dia podem ser enviadas para um determinado canal.

Confira também [limites do Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) e [requisitos de votação](/graph/api/resources/teams-api-overview#polling-requirements).

[!INCLUDE [Teams throttling documentation](../includes/throttling-teams.md)]

### <a name="identity-and-access-service-limits"></a>Limites do serviço de identidade e acesso

Os limites de serviço nesta seção se aplicam às seguintes entidades:

[!INCLUDE [Identity and access throttling documentation](../includes/throttling-identity-and-access.md)]

#### <a name="pattern"></a>Padrão

A limitação baseia-se em um algoritmo no bucket de token, que funciona adicionando custos individuais de solicitações. A soma dos custos da solicitação é depois comparada contra os limites predeterminados. Apenas as solicitações que excedem os limites serão limitadas. Se qualquer um dos limites for excedido, a resposta será `429 Too Many Requests`. É possível receber respostas `429 Too Many Requests` mesmo quando os seguintes limites não são alcançados, em situações em que os serviços estão sob uma carga importante ou com base no volume de dados para um determinado locatário. A tabela a seguir lista os limites existentes.

| Tipo de limite | Cota de unidade de recurso | Gravar cota |
| ---------- | ----------- | -------------- |
| aplicação+par de locatários | S: 3.500 solicitações por 10 segundos <br/> M: 5.000 solicitações por 10 segundos <br/> L: 8.000 solicitações por 10 segundos | 3.000 solicitações por 2 minutos e 30 segundos |
| aplicação | 150.000 solicitações por 20 segundos  | 70.000 solicitações por 5 minutos|
| locatário | Não aplicável | 18.000 solicitações por 5 minutos |

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

> [!IMPORTANT]
> 
> O custo das operações POST, PATCH e DELETE no caminho da solicitação `applications` depende do tipo **signInAudience**. Para aplicativos em que o **signInAudience** é `AzureADMyOrg` ou `AzureADMultipleOrgs`, o custo é de 70.000 solicitações por 5 minutos; enquanto para aplicativos em que o **signInAudience** é `AzureADandPersonalMicrosoftAccount` ou `PersonalMicrosoftAccount`, o custo é de 60 solicitações por minuto.

Outros fatores que afetam um custo da solicitação:

- Usar o `$select` reduz os custos por 1
- Usar o `$expand` aumenta os custos por 1
- Usar o `$top` com um valor menor que 20 reduz os custos por 1
- Criar um usuário em um locatário Azure Active Directory B2C aumenta o custo em 4

> **Observação:** Um custo da solicitação nunca pode ser menor do que 1. Qualquer custo da solicitação que se aplica a um caminho da solicitação iniciado por `me/` também se aplica a solicitações equivalentes iniciadas por `users/{id | userPrincipalName}/`.

#### <a name="additional-headers"></a>Cabeçalhos adicionais

##### <a name="request-headers"></a>Cabeçalhos de solicitação

- **x-ms-throttle-priority** - se o cabeçalho não existir ou se estiver definido com qualquer outro valor, ele indicará uma solicitação normal. Recomendamos definir a prioridade para `high` somente para as solicitações iniciadas pelo usuário. Os valores desse cabeçalho podem ser os seguintes:
  - Baixa - Indica que a solicitação tem prioridade baixa. Limitando esta solicitação não causa falhas visíveis ao usuário.
  - Normal - Padrão se nenhum valor for fornecido. Indica que a solicitação é a de prioridade padrão.
  - Alta - Indica que a solicitação é de alta prioridade. Limitando esta solicitação causa falhas visíveis ao usuário.

> **Observação:** Se as solicitações forem limitadas, as solicitações de baixa prioridade serão limitadas primeiro, as solicitações de prioridade normal em segundo e as solicitações de alta prioridade por último. Usar a prioridade no cabeçalho da solicitação não altera os limites.

##### <a name="regular-responses-requests"></a>Solicitações de respostas regulares

- **x-ms-resource-unit** - Indica a unidade de recurso usada para esta solicitação. Os valores são inteiros positivos.
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

### <a name="identity-and-access-reports-service-limits"></a>Limites do serviço de relatórios de identidade e acesso

| Tipo de solicitação |  Limitar por aplicativo por locatário |
| ------------ | ------------------------ |
| Qualquer | Cinco solicitações a cada dez segundos |

Os limites anteriores se aplicam aos seguintes recursos:

[!INCLUDE [Azure AD identity and access reports throttling documentation](../includes/throttling-aad-reports.md)]

### <a name="information-protection-service-limits"></a>Limites do serviço de proteção de informações

Os seguintes limites se aplicam a qualquer solicitação no `/informationProtection`.
  
Para o email, o recurso é um par único de mensagens de rede ID/recipiente. Por exemplo, enviar um email com o mesmo ID de mensagem enviado à mesma pessoa várias vezes em um período de 15 minutos acionará o limite por limite de recursos estabelecido na tabela a seguir. Entretanto, você pode enviar até 150 emails únicos a cada 15 minutos (limite de locatário).

| Operation                 | Limite por inquilino                                            | Limite por recurso (email, URL, arquivo)                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| POST                      | 150 solicitações a cada 15 minutos e 10000 solicitações a cada 24 horas | 1 solicitação a cada 15 minutos e 3 solicitações a cada 24 horas |

[!INCLUDE [Information protection throttling documentation](../includes/throttling-information-protection.md)]

### <a name="identity-protection-and-conditional-access-service-limits"></a>Proteção da identidade e limites do serviço de acesso condicional

| Tipo de solicitação | Limitar por locatário para todos os aplicativos |
| ------------ | ------- |
| Qualquer | 1 solicitação por segundo |

[!INCLUDE [Information protection throttling documentation](../includes/throttling-identityprotection-ca.md)]


> **Observação:** os recursos listados acima não retornam um cabeçalho `Retry-After` em respostas `429 Too Many Requests`.

### <a name="insights-service-limits"></a>Percepção dos limites de serviço

Os seguintes limites se aplicam a qualquer pedido em `me/insights` ou `users/{id}/insights`.

| Limite                                                      | Aplicável a      |
|------------------------------------------------------------|-----------------|
| 10.000 solicitações de API em um período de 10 minutos                  | pontos de extremidade v1.0 e beta |
| 4 solicitações simultâneas                                      | v1.0 e pontos finais beta   |

Os limites anteriores se aplicam aos seguintes recursos:

- [Pessoas](/graph/api/resources/people)
- [sharedInsight](/graph/api/resources/sharedinsight)
- [tendências](/graph/api/resources/trending)
- [usedInsight](/graph/api/resources/usedinsight)


### <a name="microsoft-graph-reports-service-limits"></a>Limites do serviço de relatórios do Microsoft Graph

Os seguintes limites se aplicam a qualquer solicitação no `/reports`.

| Operation                 | Limitar por aplicativo por locatário     | Limitar por locatário para todos os aplicativos |
|---------------------------|------------------------------|----------------------------|
| Qualquer pedido (CSV)         | 14 solicitações a cada 10 minutos   | 40 solicitações a cada 10 minutos |
| Qualquer solicitação (JSON, beta)  | 100 solicitações a cada 10 minutos  | n/d                        |

Os limites anteriores se aplicam individualmente a cada API de relatório. Por exemplo, uma solicitação para a API do relatório de atividades do usuário do Microsoft Teams e uma solicitação para a API do relatório de atividades do usuário do Outlook em 10 minutos contará como 1 solicitação de 14 para cada API, não 2 solicitações de 14 para ambas.

Os limites anteriores se aplicam a todos os recursos de [relatórios de uso](/graph/api/resources/report).


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

Os limites anteriores se aplicam aos seguintes recursos:[!INCLUDE [Open and schema extensions throttling documentation](../includes/throttling-extensions.md)]


### <a name="files-and-lists-service-limits"></a>Limites de serviço dos arquivos e listas

Os limites de serviço do OneDrive, OneDrive for Business e SharePoint Online não estão disponíveis. Para mais informações, confira [Por que não é possível saber o limites exatos?](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits).

As informações anteriores aplicam-se aos seguintes recursos:

[!INCLUDE [Files and lists throttling documentation](../includes/throttling-files-and-lists.md)]

### <a name="tasks-and-plans-service-limits"></a>Limites de serviços de tarefas e planos

Os limites de serviço do Planner não estão disponíveis.

As informações anteriores se aplicam aos seguintes recursos:[!INCLUDE [Tasks and plans throttling documentation](../includes/throttling-tasks-and-plans.md)]

### <a name="identity-and-access-data-policy-operation-service-limits"></a>Limites de operação de serviços de política de dados de identidade e acesso

| Tipo de solicitação | Limite por inquilino |
| ------------ | ---------------- |
| Postar no `exportPersonalData` | 1.000 solicitações por dia para todos os assuntos e 100 por assunto por dia |
| Qualquer outra solicitação | 10.000 solicitações por minuto |

Os limites anteriores se aplicam aos seguintes recursos:

- [dataPolicyOperation](/graph/api/resources/datapolicyoperation)

> **Observação:** os recursos listados acima não retornam um cabeçalho `Retry-After` nas respostas `429 Too Many Requests`.

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a>Limites do serviço de Educação

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a>Limites de serviço do Excel

Para explicações e práticas recomendadas relacionadas à limitação do serviço do Excel, veja [Limitação](workbook-best-practice.md#throttling). Além disso, a seguir estão alguns limites de limitação.
  
[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-providers-service-limits"></a>Limites de serviço dos fornecedores de identidade

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a>Limites de serviço Intune

[!INCLUDE [Intune  tunnel throttling documentation](../includes/throttling-intune-throttling-tunnel.md)]
[!INCLUDE [Intune android for work throttling documentation](../includes/throttling-intune-android-for-work.md)]
[!INCLUDE [Intune applications throttling documentation](../includes/throttling-intune-applications.md)]
[!INCLUDE [Intune auditing throttling documentation](../includes/throttling-intune-auditing.md)]
[!INCLUDE [Intune books throttling documentation](../includes/throttling-intune-books.md)]
[!INCLUDE [Intune bundles throttling documentation](../includes/throttling-intune-bundles.md)]
[!INCLUDE [Intune chromebook sync throttling documentation](../includes/throttling-intune-chromebook-sync.md)]
[!INCLUDE [Intune company terms throttling documentation](../includes/throttling-intune-company-terms.md)]
[!INCLUDE [Intune device config v2 throttling documentation](../includes/throttling-intune-device-config-v2.md)]
[!INCLUDE [Intune device configuration throttling documentation](../includes/throttling-intune-device-configuration.md)]
[!INCLUDE [Intune device enrollment throttling documentation](../includes/throttling-intune-device-enrollment.md)]
[!INCLUDE [Intune device intent throttling documentation](../includes/throttling-intune-device-intent.md)]
[!INCLUDE [Intune devices throttling documentation](../includes/throttling-intune-devices.md)]
[!INCLUDE [Intune endpoint protection throttling documentation](../includes/throttling-intune-endpoint-protection.md)]
[!INCLUDE [Intune enrollment throttling documentation](../includes/throttling-intune-enrollment.md)]
[!INCLUDE [Intune fencing throttling documentation](../includes/throttling-intune-fencing.md)]
[!INCLUDE [Intune GPAnalytics throttling documentation](../includes/throttling-intune-gpanalytics.md)]
[!INCLUDE [Intune managed applications throttling documentation](../includes/throttling-intune-managed-applications.md)]
[!INCLUDE [Intune notifications throttling documentation](../includes/throttling-intune-notifications.md)]
[!INCLUDE [Intune ODJ throttling documentation](../includes/throttling-intune-odj.md)]
[!INCLUDE [Intune partner integration throttling documentation](../includes/throttling-intune-partner-integration.md)]
[!INCLUDE [Intune rbac throttling documentation](../includes/throttling-intune-rbac.md)]
[!INCLUDE [Intune remote assistance throttling documentation](../includes/throttling-intune-remote-assistance.md)]
[!INCLUDE [Intune telephony throttling documentation](../includes/throttling-intune-telephony.md)]
[!INCLUDE [Intune TEM throttling documentation](../includes/throttling-intune-tem.md)]
[!INCLUDE [Intune troubleshooting throttling documentation](../includes/throttling-intune-troubleshooting.md)]
[!INCLUDE [Intune unlock throttling documentation](../includes/throttling-intune-unlock.md)]
[!INCLUDE [Intune updates throttling documentation](../includes/throttling-intune-updates.md)]
[!INCLUDE [Intune wip throttling documentation](../includes/throttling-intune-wip.md)]

### <a name="multi-service-limits"></a>Limites de vários serviços

[!INCLUDE [Multi tenant platform throttling documentation](../includes/throttling-multi-tenant-platform.md)]

### <a name="skype-service-limits"></a>Limites do serviço Skype

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a>Limites do serviço de assinatura

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->

### <a name="assignment-service-limits"></a>Limites de serviço de atribuição

Os limites a seguir se aplicam às solicitações no serviço de atribuição API:

| Tipo de solicitação                 | Limitar por aplicativo por locatário     | Limitar por locatário para todos os aplicativos |
|---------------------------|------------------------------|----------------------------|
| Qualquer         | 500 solicitações a cada 10 segundos   | 1000 solicitações a cada 10 segundos
|Qualquer          | 15000 solicitações a cada 3600 segundos|30000 solicitações a cada 3600 segundos|
| GET me/Assignment  | 50 solicitações a cada 10 segundos | 150 solicitações a cada 10 segundos |

Os limites anteriores se aplicam aos seguintes recursos:

- [educationAssignment](/graph/api/resources/educationassignment)
- [educationSubmission](/graph/api/resources/educationsubmission)
- [tendências](/graph/api/resources/trending)
- [educationResource](/graph/api/resources/educationresource)

### <a name="service-communications-service-limits"></a>Limites do Serviço de Comunicações
Os limites a seguir se aplicam a qualquer tipo de solicitação de comunicações de serviço em `/admin/serviceAnnouncement/`.

| Tipo de solicitação |  Limitar por aplicativo por locatário |
| ------------ | ------------------------ |
| Qualquer | 240 solicitações por 60 segundos |
|Qualquer | 800 solicitações por hora |
