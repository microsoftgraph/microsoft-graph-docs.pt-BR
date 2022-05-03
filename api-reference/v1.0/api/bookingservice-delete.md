---
title: Excluir bookingService
description: Exclua um objeto bookingService no bookingBusiness especificado.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 788895c9f09103b5b87198db6f7c974cf40ef8f8
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176851"
---
# <a name="delete-bookingservice"></a>Excluir bookingService

Namespace: microsoft.graph

[Exclua um objeto bookingService](../resources/bookingservice.md) no [bookingBusiness especificado](../resources/bookingbusiness.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  Bookings. ReadWrite.All, Bookings. Manage.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | Sem suporte.  |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
DELETE /solutions/bookingBusinesses/{id}/services/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Authorization  | Portador {código}|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.


## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

<!-- {
  "blockType": "request"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```

### <a name="response"></a>Resposta
Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


