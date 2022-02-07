---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.localizationpriority: medium
---

<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

**chatMessage** assinaturas com permissões delegadas não oferecem suporte a dados de recursos (**includeResourceData** deve ser `false`) e não requerem [criptografia](/graph/webhooks-with-resource-data). A única exceção é o recurso `/users/{id}/chats/getAllMessages` (disponível somente na versão beta) que oferece suporte a dados de recursos independentemente do tipo de permissão.

Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data). A criação de assinatura falhará se um [encryptionCertificate](/graph/api/resources/subscription) não for especificado. Antes de criar uma assinatura **chatMessage**, você deve solicitar acesso. Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).

Você deve usar o cabeçalho da solicitação `Prefer: include-unknown-enum-members` para obter os seguintes valores nos recursos **chatMessage** **messageType** [enumeração evoluível](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `systemEventMessage` para `/teams/{id}/channels/{id}/messages` e `/chats/{id}/messages`.

> [!NOTE]
>`/teams/getAllMessages`, `/chats/getAllMessages`, `/me/chats/getAllMessages` e `/users/{id}/chats/getAllMessages` tem [requisitos de licenciamento e pagamento](/graph/teams-licenses).
> `/teams/getAllMessages` e `/chats/getAllMessages` suportam ambos parâmetros de consulta `model=A` e `model=B`, `/me/chats/getAllMessages` e `/users/{id}/chats/getAllMessages` dão suporte apenas `model=B`.
> Se nenhum modelo for especificado, o [modo de avaliação](/graph/teams-licenses#evaluation-mode-default-requirements) será usado.

### <a name="conversationmember"></a>conversationMember

> [!NOTE]
>`/teams/getAllMembers` e `/chats/getAllMembers` tem [requisitos de licenciamento e pagamento](/graph/teams-licenses).
> `/teams/getAllMembers` e `/chats/getAllMembers` suportam os parâmetros de consulta `model=A` e `model=B`.
> Se nenhum modelo for especificado, o [modo de avaliação](/graph/teams-licenses#evaluation-mode-default-requirements) será usado.

#### <a name="request-example"></a>Exemplo de solicitação

Especifique o parâmetro de consulta `model` na propriedade **recurso** no corpo da solicitação.

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "chats/getAllMessages?model=A",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
