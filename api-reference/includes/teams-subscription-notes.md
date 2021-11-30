---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.localizationpriority: medium
ms.openlocfilehash: 0c2faca238d1127462de5f70aadffd1ef3edd2d0
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61132216"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

**chatMessage** assinaturas com permissões delegadas não oferecem suporte a dados de recursos (**includeResourceData** deve ser `false`) e não requerem [criptografia](/graph/webhooks-with-resource-data). A única exceção é o recurso `/users/{id}/chats/getAllMessages` (disponível somente na versão beta) que oferece suporte a dados de recursos independentemente do tipo de permissão.

Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data). A criação de assinatura falhará se um [encryptionCertificate](/graph/api/resources/subscription) não for especificado. Antes de criar uma assinatura **chatMessage**, você deve solicitar acesso. Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).

> [!NOTE]
>`/teams/getAllMessages`e `/chats/getAllMessages` tem [requisitos de licenciamento e pagamento.](/graph/teams-licenses)
> `/teams/getAllMessages` e `/chats/getAllMessages` dar suporte a `model=A` `model=B` parâmetros de consulta e.
> Se nenhum modelo for especificado, o [modo de avaliação](/graph/teams-licenses#evaluation-mode-default-requirements) será usado.

### <a name="conversationmember"></a>conversationMember

> [!NOTE]
>`/teams/getAllMembers`e `/chats/getAllMembers` tem [requisitos de licenciamento e pagamento.](/graph/teams-licenses)
> `/teams/getAllMembers` e `/chats/getAllMembers` dar suporte a `model=A` `model=B` parâmetros de consulta e.
> Se nenhum modelo for especificado, o [modo de avaliação](/graph/teams-licenses#evaluation-mode-default-requirements) será usado.

### <a name="request-example"></a>Exemplo de solicitação

`model`Especifique o parâmetro de consulta na propriedade **resource** no corpo da solicitação.

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
