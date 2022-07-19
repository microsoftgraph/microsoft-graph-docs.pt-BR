---
title: Listar ediscoveryNoncustodialDataSources
description: Obtenha uma lista de objetos ediscoveryNoncustodialDataSource.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: e1a49e58687c5cafb16eb7e11ebd495a395b60da
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838343"
---
# <a name="list-ediscoverynoncustodialdatasources"></a>Listar ediscoveryNoncustodialDataSources
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista das [fontes de dados não custodiais](../resources/security-ediscoverynoncustodialdatasource.md) e suas propriedades.

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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/noncustodialDataSources
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este `200 OK` método retornará um código de resposta e uma coleção do objeto [microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_ediscoverynoncustodialdatasource_from_"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialdatasources?$expand=dataSource
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-ediscoverynoncustodialdatasource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-ediscoverynoncustodialdatasource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-ediscoverynoncustodialdatasource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-ediscoverynoncustodialdatasource-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryNoncustodialDataSource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/noncustodialDataSources(dataSource())",
    "@odata.count": 3,
    "value": [
        {
            "status": "active",
            "holdStatus": "applied",
            "createdDateTime": "2022-05-23T02:09:11.1395287Z",
            "lastModifiedDateTime": "2022-05-23T02:09:11.1395287Z",
            "releasedDateTime": "0001-01-01T00:00:00Z",
            "id": "35393639323133394345384344303043",
            "displayName": "U.S. Sales",
            "dataSource@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/noncustodialDataSources('35393639323133394345384344303043')/dataSource/$entity",
            "dataSource": {
                "@odata.type": "#microsoft.graph.security.siteSource",
                "@odata.id": "https://graph.microsoft.com/v1.0/sites/169718e3-a8df-449d-bef4-ee09fe1ddc5d",
                "displayName": "U.S. Sales",
                "createdDateTime": "2022-05-23T02:09:11.1395535Z",
                "holdStatus": "0",
                "id": "169718e3-a8df-449d-bef4-ee09fe1ddc5d",
                "createdBy": {
                    "application": null,
                    "user": {
                        "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                        "displayName": null
                    }
                },
                "site": {
                    "webUrl": "https://m365x809305.sharepoint.com/sites/USSales",
                    "id": "169718e3-a8df-449d-bef4-ee09fe1ddc5d",
                    "createdDateTime": "2022-05-23T02:09:11.1395535Z"
                }
            }
        },
        {
            "status": "active",
            "holdStatus": "applied",
            "createdDateTime": "2022-05-23T02:09:11.1395287Z",
            "lastModifiedDateTime": "2022-05-23T02:09:11.1395287Z",
            "releasedDateTime": "0001-01-01T00:00:00Z",
            "id": "31453237353743363432414242344641",
            "displayName": "Sales and Marketing",
            "dataSource@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/noncustodialDataSources('31453237353743363432414242344641')/dataSource/$entity",
            "dataSource": {
                "@odata.type": "#microsoft.graph.security.siteSource",
                "@odata.id": "https://graph.microsoft.com/v1.0/sites/74f6c798-fc32-4dbe-9e5b-8e11459b9f44",
                "displayName": "Sales and Marketing",
                "createdDateTime": "2022-05-23T02:09:11.1397925Z",
                "holdStatus": "0",
                "id": "74f6c798-fc32-4dbe-9e5b-8e11459b9f44",
                "createdBy": {
                    "application": null,
                    "user": {
                        "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                        "displayName": null
                    }
                },
                "site": {
                    "webUrl": "https://m365x809305.sharepoint.com/sites/SalesAndMarketing",
                    "id": "74f6c798-fc32-4dbe-9e5b-8e11459b9f44",
                    "createdDateTime": "2022-05-23T02:09:11.1397925Z"
                }
            }
        },
        {
            "status": "active",
            "holdStatus": "applied",
            "createdDateTime": "2022-05-23T02:09:11.1395287Z",
            "lastModifiedDateTime": "2022-05-23T02:09:11.1395287Z",
            "releasedDateTime": "0001-01-01T00:00:00Z",
            "id": "46333131344239353834433430454335",
            "displayName": "Retail",
            "dataSource@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/noncustodialDataSources('46333131344239353834433430454335')/dataSource/$entity",
            "dataSource": {
                "@odata.type": "#microsoft.graph.security.siteSource",
                "@odata.id": "https://graph.microsoft.com/v1.0/sites/dbe4b18e-2765-4989-8647-48139180c45f",
                "displayName": "Retail",
                "createdDateTime": "2022-05-23T02:09:11.1399861Z",
                "holdStatus": "0",
                "id": "dbe4b18e-2765-4989-8647-48139180c45f",
                "createdBy": {
                    "application": null,
                    "user": {
                        "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                        "displayName": null
                    }
                },
                "site": {
                    "webUrl": "https://m365x809305.sharepoint.com/sites/Retail",
                    "id": "dbe4b18e-2765-4989-8647-48139180c45f",
                    "createdDateTime": "2022-05-23T02:09:11.1399861Z"
                }
            }
        }
    ]
}
```

