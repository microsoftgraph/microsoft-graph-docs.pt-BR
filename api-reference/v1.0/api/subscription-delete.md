---
title: Excluir assinatura
description: Exclua uma assinatura.
ms.openlocfilehash: 249393cef11e2768eec0a6435a8485b51cf6921c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007316"
---
# <a name="delete-subscription"></a>Excluir assinatura

Exclua uma assinatura.

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
|Alerta de segurança| SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
