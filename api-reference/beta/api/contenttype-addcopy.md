---
author: swapnil1993
title: 'contentType: addCopy'
description: Adicione uma cópia de um tipo de conteúdo de site a uma lista.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: b6a75c30368535396e69f917f50a76c4234eb58c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344590"
---
# <a name="contenttype-addcopy"></a>contentType: addCopy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Adicione uma cópia de um tipo [de conteúdocontentType] de um [site][site] a uma [lista][list].[]
 
  

## <a name="permissions"></a>Permissões  

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

  

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |Sites.Manage.All, Sites.FullControl.All  |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo | Sites.Manage.All, Sites.FullControl.All |

  

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/{site-id}/lists/{list-id}/contentTypes/addCopy
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|-|-|-|
|contentType| cadeia de caracteres | URL canônica para o tipo de conteúdo do site que será copiado para a lista. Obrigatório.|

## <a name="response"></a>Resposta

Se tiver êxito, essa chamada retornará um `201 Created` código de resposta e um [objeto contentType][] no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_addcopy"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/contentTypes/addCopy
Content-Type: application/json

{
  "contentType": "https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-addcopy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-addcopy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-addcopy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-addcopy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/contenttype-addcopy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/contenttype-addcopy-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a>Resposta


<!-- { "blockType": "response", "@type": "microsoft.graph.contentType", "truncated": true} -->

```http
HTTP/1.1 201 Created

{
    "id": "0x0101",
    "description": "Create a new custom CSR JavaScript Display Template.",
    "group": "Display Template Content Types",
    "hidden": false,
    "name": "JavaScript Display Template",
    "parentId": "0x01",
    "readOnly": false,
    "sealed": false,
    "base": {
        "id": "0x01",
        "description": "Create a new custom CSR JavaScript Display Template.",
        "group": "Display Template Content Types",
        "hidden": false,
        "name": "JavaScript Display Template",
        "readOnly": false,
        "sealed": false
    }
}
```

[site]: ../resources/site.md
[list]: ../resources/list.md
[contentType]: ../resources/contentType.md
