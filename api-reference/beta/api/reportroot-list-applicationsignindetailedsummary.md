---
title: Listar applicationSignInDetailedSummary
description: Recupere os objetos applicationSignInDetailedSummary.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 2e9a7ddbe89b6b068a0c90d9833975c32e538a3b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096094"
---
# <a name="list-applicationsignindetailedsummary"></a>Listar applicationSignInDetailedSummary
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere [os objetos applicationSignInDetailedSummary.](../resources/applicationsignindetailedsummary.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Reports.Read.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/applicationSignInDetailedSummary
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos `$filter` `$top` parâmetros de consulta E OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_applicationsignindetailedsummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-applicationsignindetailedsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-applicationsignindetailedsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-applicationsignindetailedsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-applicationsignindetailedsummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-applicationsignindetailedsummary-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-applicationsignindetailedsummary-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.applicationSignInDetailedSummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#reports/applicationSignInDetailedSummary",
    "value": [
        {
            "id": "ce0d6f77-04d2-49f6-bfcc-ad101cd4b69f",
            "appId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "appDisplayName": "Graph Explorer",
            "aggregatedEventDateTime": "2021-12-28T00:00:00Z",
            "signInCount": 5,
            "status": {
                "errorCode": 0,
                "failureReason": null,
                "additionalDetails": null
            }
        },
        {
            "id": "59397b28-0dc5-4270-b869-24714ea4aedb",
            "appId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "appDisplayName": "Graph Explorer",
            "aggregatedEventDateTime": "2021-12-06T00:00:00Z",
            "signInCount": 5,
            "status": {
                "errorCode": 650057,
                "failureReason": "Invalid resource. The client has requested access to a resource which is not listed in the requested permissions in the client's application registration. Client app ID: {appId}({appName}). Resource value from request: {resource}. Resource app ID: {resourceAppId}. List of valid resources from app registration: {regList}.",
                "additionalDetails": null
            }
        },
        {
            "id": "29d5acee-e7c8-4565-96eb-f89719cb4d9f",
            "appId": "c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
            "appDisplayName": "Azure Portal",
            "aggregatedEventDateTime": "2021-12-28T00:00:00Z",
            "signInCount": 1,
            "status": {
                "errorCode": 0,
                "failureReason": null,
                "additionalDetails": null
            }
        },
        {
            "id": "88348b99-6c59-47db-bc70-2011d80e3bd6",
            "appId": "89bee1f7-5e6e-4d8a-9f3d-ecd601259da7",
            "appDisplayName": "Office365 Shell WCSS-Client",
            "aggregatedEventDateTime": "2021-11-30T00:00:00Z",
            "signInCount": 3,
            "status": {
                "errorCode": 0,
                "failureReason": null,
                "additionalDetails": null
            }
        }
    ]
}
```
