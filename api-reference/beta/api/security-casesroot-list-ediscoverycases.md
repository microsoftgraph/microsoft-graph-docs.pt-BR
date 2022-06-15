---
title: Listar ediscoveryCases
description: Obter uma lista dos casos de Descoberta Eletrônica
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: dd70dbb010fcdfff5aa8e90cc88ff3714a8f75e9
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092482"
---
# <a name="list-ediscoverycases"></a>Listar ediscoveryCases
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista dos [objetos ediscoveryCase](../resources/security-ediscoverycase.md) e suas propriedades.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/cases/ediscoveryCases
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `200 OK` um código de resposta e uma coleção [de objetos ediscoveryCase](../resources/security-ediscoverycase.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_ediscoverycase"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/ediscoveryCases
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-ediscoverycase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-ediscoverycase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-ediscoverycase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-ediscoverycase-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
A seguir está um exemplo da resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.ediscoveryCase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases",
    "@odata.count": 22,
    "value": [
        {
            "description": "",
            "lastModifiedDateTime": "2022-05-19T23:30:41.23Z",
            "status": "active",
            "closedDateTime": null,
            "externalId": "",
            "id": "60f86305-ac3e-408b-baa2-ea585dd8b0c0",
            "displayName": "My case 1",
            "createdDateTime": "2022-05-19T23:30:41.23Z",
            "lastModifiedBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": "MOD Administrator"
                }
            },
            "closedBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": ""
                }
            }
        },
        {
            "description": "",
            "lastModifiedDateTime": "2022-05-18T23:05:07.82Z",
            "status": "active",
            "closedDateTime": null,
            "externalId": "",
            "id": "7acdda75-3559-4f93-9827-cbd4c89db033",
            "displayName": "My case 2",
            "createdDateTime": "2022-05-18T23:05:07.82Z",
            "lastModifiedBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": "MOD Administrator"
                }
            },
            "closedBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": ""
                }
            }
        }
    ]
}
```

