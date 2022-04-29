---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.localizationpriority: medium
ms.openlocfilehash: 6e5f62d52969dcc1b332b2cd6e5f02f318c8b6a9
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65135142"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

**chatMessage** assinaturas podem ser especificadas para incluir dados de recurso. Se especificado para incluir dados de recurso (**includeResourceData** definido como `true`), [encryption](/graph/webhooks-with-resource-data) é necessária. A criação de assinatura falhará se um [encryptionCertificate](/graph/api/resources/subscription) não for especificado para tais assinaturas. Antes de criar uma assinatura **chatMessage** com permissões de aplicativo, talvez seja necessário solicitar acesso. Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).

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
