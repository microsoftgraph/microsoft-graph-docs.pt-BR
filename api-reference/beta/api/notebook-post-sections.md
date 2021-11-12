---
title: Criar seção
description: Crie uma nova seção no bloco de anotações especificado.
author: jewan-microsoft
ms.localizationpriority: medium
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 350bc1699f57256ff2385939c624c7712c8744ac
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60941236"
---
# <a name="create-section"></a>Criar seção

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie uma nova [seção](../resources/onenotesection.md) no bloco de anotações especificado.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Notes.Create, Notes.ReadWrite    |
|Aplicativo | Notes.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sections
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
POST /groups/{id}/onenote/notebooks/{id}/sections
POST /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-Type | string | `application/json` |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça um nome para a seção.

Dentro do mesmo nível de hierarquia, os nomes das seções devem ser exclusivos. O nome não pode conter mais de 50 caracteres ou conter os seguintes caracteres:  ?*\/:<>|&#''%~

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [onenoteSection](../resources/onenotesection.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_section_from_notebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sections
Content-type: application/json

{
  "displayName": "Section name"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-section-from-notebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-section-from-notebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-section-from-notebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-section-from-notebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


