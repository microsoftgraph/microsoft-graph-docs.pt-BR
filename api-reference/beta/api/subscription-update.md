---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 19355ff8acbcdade689b140abca63e8d9885e3fc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512777"
---
# <a name="update-subscription"></a>Atualizar assinatura

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Renove uma assinatura ampliando seu tempo de validade.

Assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso. Para evitar notificações de ausentes, um aplicativo deve renovar suas assinaturas bem antes de começar sua data de expiração. Consulte [assinatura](../resources/subscription.md) para o comprimento máximo de uma assinatura para cada tipo de recurso.

## <a name="permissions"></a>Permissões

A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de recurso/item        | Permissão          |
|-----------------------------|---------------------|
| Contatos                    | Contacts.Read       |
| Conversas               | Group.Read.All      |
| Eventos                      | Calendars.Read      |
| Mensagens                    | Mail.Read           |
| Grupos                      | Group.Read.All      |
| Usuários                       | User.Read.All       |
| Drive (o OneDrive do usuário)    | Files.ReadWrite     |
| Drives (conteúdo do SharePoint shared e unidades) | Files.ReadWrite.All |
|Alerta de segurança               | SecurityEvents.ReadWrite.All |

***Observação:*** O ponto de extremidade /beta permite que as permissões de aplicativo para a maioria dos recursos. Não há suporte para conversas em itens de raiz uma unidade OneDrive e de grupo com permissões de aplicativo.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
