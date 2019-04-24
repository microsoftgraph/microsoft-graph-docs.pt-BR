---
title: Configurar notificações para alterações nos dados de usuário
description: A API do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 7060a1d6f213a413c453725774da8ffeedb1b277
ms.sourcegitcommit: d264fa064215879fa88a4680402cd57a470d73db
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2019
ms.locfileid: "31980932"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a>Configurar notificações para alterações nos dados de usuário

A API do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.

Depois que o Microsoft Graph aceita a solicitação de assinatura, ele envia notificações por push para a URL especificada na assinatura. O aplicativo então realiza ações de acordo com sua lógica comercial. Por exemplo, ele busca mais dados, atualiza o cache e as exibições, etc.

## <a name="supported-resources"></a>Recursos com suporte

Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:

- [Mensagem][] do Outlook
- [Evento][] do Outlook
- [Contato][] pessoal do Outlook
- [user][]
- [group][]
- [Conversa][] em grupo do Office 365
- Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _qualquer pasta_ no OneDrive pessoal do usuário
- Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _pasta raiz_ no OneDrive for Business
- [Alerta][] de segurança

Você pode criar uma assinatura para uma pasta de específica do Outlook, como a Caixa de Entrada: `me/mailFolders('inbox')/messages`

Ou para um recurso de nível superior: `me/messages`, `me/contacts`, `me/events`, `users` ou `groups`

Ou para uma instância de recurso específica: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`

Ou para alguma pasta no OneDrive pessoal de um usuário: `/drives/{id}/root`
`/drives/{id}/root/subfolder`

Ou para a pasta raiz de uma unidade do SharePoint/OneDrive for Business: `/drive/root`

Ou para um novo alerta da [API de Segurança](security-concept-overview.md): `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`

### <a name="azure-ad-resource-limitations"></a>Limitações de recursos do Microsoft Azure AD

Determinadas limites se aplicam aos recursos baseados no Azure AD (usuários, grupos) e gerarão erros se forem excedidos:

> **Observação**: Esses limites não se aplicam aos recursos de serviços diferente do Azure AD. Por exemplo, um aplicativo pode criar muito mais assinaturas para `message` ou recursos `event` que são aceitos pelo serviço Exchange Online como parte do Microsoft Graph.

- Cotas máximas de assinaturas:

  - Por aplicativo: total de 50 mil assinaturas
  - Por locatário: total de 1000 assinaturas em todos os aplicativos
  - Combinação por aplicativo e locatário: 100 assinaturas no total

Quando os limites são excedidos, a tentativa de criar uma assinatura resultará em uma [resposta de erro](errors.md) - `403 Forbidden`. A propriedade `message` explicará qual limite foi excedido.

- Não há suporte a locatários do Microsoft Azure AD B2C.

- Não há suporte a notificações para entidades de usuário para contas Microsoft pessoais.

## <a name="subscription-lifetime"></a>Tempo de vida da assinatura

As assinaturas têm tempo de vida limitado. Os aplicativos precisam renovar suas assinaturas antes do tempo de expiração. Caso contrário, será preciso criar uma nova assinatura. Confira a lista de prazos máximos em [Prazo máximo de assinatura por tipo de recurso](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).

Os aplicativos também podem cancelar a assinatura a qualquer momento para deixarem de receber notificações.

## <a name="managing-subscriptions"></a>Gerenciar assinaturas

Os clientes podem criar, renovar e excluir assinaturas.

### <a name="creating-a-subscription"></a>Criar uma assinatura

Criar uma assinatura é a primeira etapa para começar a receber notificações de um recurso. O processo de assinatura ocorre da seguinte maneira:

1. O cliente envia uma solicitação de assinatura (POST) para um recurso específico.

1. O Microsoft Graph verifica a solicitação.

    - Se a solicitação for válida, o Microsoft Graph enviará um token de validação para a URL de notificação.
    - Se a solicitação for inválida, o Microsoft Graph enviará uma resposta de erro com um código e detalhes.

1. O cliente envia o token de validação de volta para o Microsoft Graph.

1. O Microsoft Graph envia uma resposta de volta para o cliente.

O cliente deve armazenar a ID da assinatura para correlacionar notificações com a assinatura.

#### <a name="subscription-request-example"></a>Exemplo de solicitação de assinatura

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/notificationClient",
  "resource": "/me/mailfolders('inbox')/messages",
  "expirationDateTime": "2016-03-20T11:00:00.0000000Z",
  "clientState": "SecretClientState"
}
```

As propriedades `changeType`, `notificationUrl`, `resource` e `expirationDateTime` são obrigatórias. Confira os valores e as definições de propriedade em [tipo de recurso de assinatura](/graph/api/resources/subscription?view=graph-rest-1.0).

A propriedade `resource` especifica o recurso que será monitorado para detectar alterações. Por exemplo, você pode criar uma assinatura para uma pasta de email específica: `me/mailFolders('inbox')/messages` ou em nome de um usuário, atribuído com uma autorização do administrador: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.

Embora a `clientState` não seja obrigatória, você deve incluí-la para manter a conformidade com nosso processo recomendado de manipulação de notificações. A definição desta propriedade permitirá confirmar se as notificações recebidas partirão do serviço do Microsoft Graph. Por esse motivo, o valor da propriedade deve continuar em segredo e deve ser conhecido somente por seu aplicativo e pelo serviço do Microsoft Graph.

Se tiver êxito, o Microsoft Graph retornará um código `201 Created` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo.

#### <a name="notification-endpoint-validation"></a>Validação de ponto de extremidade de notificação

O Microsoft Graph valida o ponto de extremidade de notificação fornecido na propriedade `notificationUrl` da solicitação de assinatura antes de criar a assinatura. O processo de validação ocorre da seguinte maneira:

1. O Microsoft Graph envia uma solicitação POST para a URL de notificação:

    ``` http
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > **Importante:** como `validationToken` é um parâmetro de consulta, ele deve ser decodificado corretamente pelo cliente, de acordo com as práticas de codificação HTTP. Se o cliente não decodificar o token e usar o valor codificado na próxima etapa (resposta), a validação falhará. Além disso, o cliente deve tratar o valor de token como opaco, pois o formato de token pode ser alterado no futuro, sem aviso prévio.

1. O cliente deve fornecer uma resposta com as seguintes características em até 10 segundos:

    - Um código de status 200 (OK).
    - O tipo de conteúdo deve ser `text/plain`.
    - O corpo deve incluir o token de validação fornecido pelo Microsoft Graph.

O cliente deve descartar o token de validação depois de o fornecer na resposta.

### <a name="renewing-a-subscription"></a>Renovar uma assinatura

O cliente pode renovar uma assinatura com uma data de expiração específica de até três dias desde a hora da solicitação. A propriedade `expirationDateTime` é obrigatória.

#### <a name="subscription-renewal-example"></a>Exemplo de renovação de assinatura

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

Se tiver êxito, o Microsoft Graph retornará um código `200 OK` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo. O objeto subscription inclui o novo valor de `expirationDateTime`.

### <a name="deleting-a-subscription"></a>Excluindo uma assinatura

O cliente pode parar de receber notificações excluindo a assinatura com o uso de sua ID.

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

Se tiver êxito, o Microsoft Graph retornará um código `204 No Content`.

## <a name="notifications"></a>Notificações

O cliente começa a receber notificações depois de criar a assinatura. O Microsoft Graph envia uma solicitação POST à URL de notificação quando o recurso é alterado. Notificações são enviadas somente para as alterações do tipo especificado na assinatura, por exemplo, `created`.

> **Observação:** ao usar várias assinaturas que monitoram o mesmo tipo de recurso e usam a mesma URL de notificação, é possível enviar uma solicitação POST incluindo várias notificações com IDs de assinatura diferentes. Não há garantias de que todas as notificações na solicitação POST pertencerão a uma única assinatura.

### <a name="notification-properties"></a>Propriedades do objeto notification

O objeto notification tem as seguintes propriedades:

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| subscriptionId | string | A ID da assinatura que gerou a notificação. |
| subscriptionExpirationDateTime | [dateTime](https://tools.ietf.org/html/rfc3339) | O tempo de expiração da assinatura. |
| clientState | string | A propriedade `clientState` especificada na solicitação de assinatura. (caso haja). |
| changeType | string | O tipo de evento que gerou a notificação. Por exemplo, `created` ao receber um email ou `updated` ao marcar uma mensagem como lida. |
| recurso | string | O URI do recurso relativo a `https://graph.microsoft.com`. |
| resourceData | objeto | O conteúdo dessa propriedade depende do tipo de recurso que está sendo assinado. |

Por exemplo, para recursos do Outlook, `resourceData` contém os seguintes campos:

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| @odata.type | string | O tipo de entidade OData no Microsoft Graph que descreve o objeto representado. |
| @odata.id | string | O identificador OData do objeto. |
| @odata.etag | string | A marca da entidade HTTP que representa a versão do objeto. |
| id | string | O identificador do objeto. |

> **Observação** O valor de `id` fornecido em `resourceData` é válido no momento em que a notificação é gerada. Algumas ações, como mover uma mensagem para outra pasta, podem fazer com que o `id` não seja mais válido quando a notificação for processada.

### <a name="notification-example"></a>Exemplo de notificação

Quando o usuário recebe um email, o Microsoft Graph envia uma notificação semelhante à seguinte:

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@<tenant_guid>/messages/{long_id_string}",
      "resourceData":
      {
        "@odata.type":"#Microsoft.Graph.Message",
        "@odata.id":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
        "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
        "id":"<long_id_string>"
      }
    }
  ]
}
```

Observe que o campo `value` é uma matriz de objetos. Quando houver muitas notificações na fila, o Microsoft Graph poderá enviar vários itens em uma única solicitação. Notificações de diferentes assinaturas podem ser incluídas na mesma solicitação de notificação.

### <a name="processing-the-notification"></a>Processar a notificação

Cada notificação recebida por seu aplicativo deve ser processada. Estas são as tarefas mínimas que o seu aplicativo deve realizar para processar uma notificação:

1. Validar a propriedade `clientState`. Ela deve corresponder ao valor enviado originalmente com a solicitação de criação da assinatura.

    > **Observação:** se isso não for verdadeiro, você não deverá considerar esta notificação como válida. É possível que a notificação não tenha se originado do Microsoft Graph e possa ter sido enviada por um ator invasor. Você também deve investigar de onde vem a notificação e tomar as medidas apropriadas.

1. Atualize seu aplicativo com base na sua lógica comercial.

1. Envie um código de status `202 - Accepted` na sua resposta para o Microsoft Graph. Se o Microsoft Graph não receber um código de classe 2xx, ele tentará reenviar a notificação várias vezes.

    > **Observação:** você deve enviar um código de status `202 - Accepted` mesmo que a propriedade `clientState` não corresponda àquela enviada com a solicitação de assinatura. Essa é uma boa prática, uma vez que impede que um possível ator invasor descubra que você não confia nas notificações dele e use as informações para tentar adivinhar o valor da propriedade `clientState`.

Repita o procedimento para outras notificações na solicitação.

## <a name="code-samples"></a>Exemplos de código

Os exemplos de código a seguir estão disponíveis no GitHub.

- [Exemplo de webhooks do Microsoft Graph para Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [Exemplo de webhooks do Microsoft Graph para ASP.NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [Exemplo de webhooks de usuários do Microsoft Graph usando o SDK do WebJobs](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a>Confira também

- [Tipo de recurso de assinatura](/graph/api/resources/subscription?view=graph-rest-1.0)
- [Obter assinatura](/graph/api/subscription-get?view=graph-rest-1.0)
- [Criar assinatura](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)

[contato]: /graph/api/resources/contact?view=graph-rest-1.0
[conversa]: /graph/api/resources/conversation?view=graph-rest-1.0
[driveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[group]: /graph/api/resources/group?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
[user]: /graph/api/resources/user?view=graph-rest-1.0
[alert]: /graph/api/resources/alert?view=graph-rest-1.0
