---
author: swapnil1993
title: Atualizar contentType
description: Atualize um tipo de conteúdo.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 78be26b9e0804565bc02f2f95e6964837bc96395
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134087"
---
# <a name="update-contenttype"></a>Atualizar contentType
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Atualizar um [tipo de conteúdo][contentType].
  

## <a name="permissions"></a>Permissões

  

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

  

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.Manage.All, Sites.FullControl.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo |Sites.Manage.All, Sites.FullControl.All |

  

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /sites/{site-id}/contentTypes/{contentType-id}
PATCH /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [recurso contentType][] a ser atualizado.  

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto contentType][] atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contenttype"
}
-->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}
Content-Type: application/json

{
   "name":"updatedCt",
   "documentSet":{
      "shouldPrefixNameToFile":true,
      "allowedContentTypes":[
         {
            "id":"0x0101",
            "name":"Document"
         }
      ],
      "defaultContents":[
         {
            "fileName":"a.txt",
            "contentType":{
               "id":"0x0101"
            }
         },
         {
            "fileName":"b.txt",
            "contentType":{
               "id":"0x0101"
            }
         }
      ],
      "sharedColumns":[
         {
            "name":"Description",
            "id":"cbb92da4-fd46-4c7d-af6c-3128c2a5576e"
         },
         {
            "name":"Address",
            "id":"fc2e188e-ba91-48c9-9dd3-16431afddd50"
         }
      ],
      "welcomePageColumns":[
         {
            "name":"Address",
            "id":"fc2e188e-ba91-48c9-9dd3-16431afddd50"
         }
      ]
   }
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-contenttype-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-contenttype-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- { "blockType": "response", "@type": "microsoft.graph.contentType", "truncated": true} -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "id":"0x0101009B237E76EF94DC49B4E58139041E7C60",
   "description":"",
   "eTag":"\"7\"",
   "group":"Custom Content Types",
   "hidden":false,
   "name":"testdoc",
   "parentId":"0x0101",
   "base":{
      "id":"0x0101",
      "name":"Document"
   }
}
```

[contentType]: ../resources/contentType.md
