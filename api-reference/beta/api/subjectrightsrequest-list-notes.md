---
title: Listar anotações
description: Obtenha os recursos authoredNote da propriedade de navegação de anotações.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: e1a934f721f079699e63920e58e62d551d4e1534
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461538"
---
# <a name="list-notes"></a>Listar anotações
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha a lista de anotações autoradas associadas a uma solicitação de direitos de assunto. 

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|SubjectRightsRequest.Read.All, SubjectRightsRequest.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte|

## <a name="http-request"></a>Solicitação HTTP

[!INCLUDE [subject-rights-request-privacy-deprecate](../../includes/subject-rights-request-privacy-deprecate.md)]

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/subjectRightsRequests/{subjectRightsRequestId}/notes
GET /privacy/subjectRightsRequests/{subjectRightsRequestId}/notes
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método não dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `200 OK` de resposta e uma coleção de [objetos authoredNote](../resources/authorednote.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_authorednote"
}
-->
``` http
GET https://graph.microsoft.com/beta/privacy/subjectRightsRequests/{subjectRightsRequestId}/notes
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-authorednote-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-authorednote-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-authorednote-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-authorednote-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-authorednote-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.authoredNote)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/privacy/subjectRightsRequests('77f885ac-1d7b-4317-bde8-4cb3d24a3ed8')/notes",
    "value": [
        {
            "id": "73A1E594-D973-4740-B1CC-42FD21727543",
            "createdDateTime": "2022-06-20T22:42:28Z",
            "author": {
                "user": {
                    "id": "1B761ED2-AA7E-4D82-9CF5-C09D737B6167",
                    "displayName": "srradmin@contoso.com"
                }
            },
            "content": {
                "content": "Please review all the files tagged with follow up.",
                "contentType": "text"
            }
        }
    ]
}
```

