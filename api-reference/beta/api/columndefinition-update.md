---
author: swapnil1993
title: Atualizar columnDefinition
description: Atualizar uma coluna de site, lista ou tipo de conteúdo
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 0c8e888214007288e9e6ba8df8e9815b127bec02
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975611"
---
# <a name="update-columndefinition"></a>Atualizar columnDefinition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Atualizar um [site,][] [lista ou][] [tipo de conteúdo.][contentType] [column][columnDefinition]
  

## <a name="permissions"></a>Permissões  

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

  

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.Manage.All, Sites.FullControl.All  |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo | Sites.Manage.All, Sites.FullControl.All |

  

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /sites/{site-id}/columns/{column-id}
PATCH /sites/{site-id}/lists/{list-id}/columns/{column-id}
PATCH /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
PATCH /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```


## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|


## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON dessas propriedades de um [recurso columnDefinition][] a ser atualizado. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

Para colunas no **site** ou **lista**, você pode atualizar qualquer propriedade **de columnDefinition** diferente da **propriedade id.**

Para colunas em **contentType**, você pode atualizar apenas **a propriedade necessária** **ou** oculta.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [columnDefinition][] atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contenttype_column"
}
-->
```http
PATCH /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
Content-Type: application/json

{
  "required": true,
  "hidden": false,
  "propagateChanges": false     
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contenttype-column-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contenttype-column-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contenttype-column-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contenttype-column-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-contenttype-column-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.columnDefinition"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Custom Column",
  "enforceUniqueValues": false,
  "hidden": false,
  "id": "11dfef35-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Custom Column",
  "readOnly": false,
  "required": true,
  "text": {
    "allowMultipleLines": false,
    "appendChangesToExistingText": false,
    "linesForEditing": 0,
    "maxLength": 255
  }
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[contentType]: ../resources/contentType.md
[list]: ../resources/list.md
[site]: ../resources/site.md

