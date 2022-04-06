---
title: Listar servicePrincipalRiskDetections
description: Recupere as propriedades de uma coleção de objetos servicePrincipalRiskDetection.
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d9fc67aa8a0b8db0efd2db016392b790e43ebfe3
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510341"
---
# <a name="list-serviceprincipalriskdetections"></a>Listar servicePrincipalRiskDetections
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades de uma coleção de [objetos servicePrincipalRiskDetection](../resources/serviceprincipalriskdetection.md) .

>**Observação:** Você deve ter uma Azure AD Premium P1 ou P2 para usar a API servicePrincipalRiskDetection.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|IdentityRiskEvent.Read.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|IdentityRiskEvent.Read.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/servicePrincipalRiskDetections
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos parâmetros `$filter` `$select` de consulta E OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de [objetos servicePrincipalRiskDetection](../resources/serviceprincipalriskdetection.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-list-risk-detections"></a>Exemplo 1: Listar detecções de risco

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceprincipalriskdetection"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityProtection/servicePrincipalRiskDetections
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceprincipalriskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceprincipalriskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceprincipalriskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceprincipalriskdetection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-serviceprincipalriskdetection-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta

Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.servicePrincipalRiskDetection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
    "@odata.type": "#microsoft.graph.servicePrincipalRiskDetection",
    "id": "2856d6e87c5c3a74021ff70291fa68107570c150d8dc145bdea5",
    "requestId": null,
    "correlationId": null,
    "riskEventType": "investigationsThreatIntelligence",
    "riskState": "atRisk",
    "riskLevel": "high",
    "riskDetail": "none",
    "source": "IdentityProtection",
    "detectionTimingType": "offline",
    "activity": "servicePrincipal",
    "tokenIssuerType": "AzureAD",
    "ipAddress": null,
    "location": null,
    "activityDateTime": "2021-10-26T00:00:00Z",
    "detectedDateTime": "2021-10-26T00:00:00Z",
    "lastUpdatedDateTime": "2021-10-26T16:28:17.8202975Z)",
    "servicePrincipalId": "99b8d28b-11ae-4e84-9bef-0e767e286grg",
    "servicePrincipalDisplayName": "Contoso App",
    "appId": "0grb38ac-a572-491d-a9db-b07197643457",
    "keyIds": [
      "9d9fea30-d8e3-481b-b57c-0ef569a989e5"
    ],
    "additionalInfo": "[{\"Key\":\"alertUrl\",\"Value\":null}]"
    }
  ]
}
```

### <a name="example-2-list-risk-detections-and-filter-the-results"></a>Exemplo 2: Listar detecções de risco e filtrar os resultados

#### <a name="request"></a>Solicitação
O exemplo a seguir mostra como usar para `$filter` `medium` obter a coleção de detecções de risco principal do serviço onde o nível de risco está ou o tipo de evento de risco é `investigationsThreatIntelligence`.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_serviceprincipalriskdetection"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityProtection/servicePrincipalRiskDetections?$filter=riskEventType eq 'investigationsThreatIntelligence' or riskLevel eq 'medium'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-serviceprincipalriskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-serviceprincipalriskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-serviceprincipalriskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-filter-serviceprincipalriskdetection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-filter-serviceprincipalriskdetection-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.servicePrincipalRiskDetection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
    "@odata.type": "#microsoft.graph.servicePrincipalRiskDetection",
    "id": "2856d6e87c5c3a74021ff70291fa68107570c150d8dc145bdea5",
    "requestId": null,
    "correlationId": null,
    "riskEventType": "investigationsThreatIntelligence",
    "riskState": "atRisk",
    "riskLevel": "high",
    "riskDetail": "none",
    "source": "IdentityProtection",
    "detectionTimingType": "offline",
    "activity": "servicePrincipal",
    "tokenIssuerType": "AzureAD",
    "ipAddress": null,
    "location": null,
    "activityDateTime": "2021-10-26T00:00:00Z",
    "detectedDateTime": "2021-10-26T00:00:00Z",
    "lastUpdatedDateTime": "2021-10-26T16:28:17.8202975Z)",
    "servicePrincipalId": "99b8d28b-11ae-4e84-9bef-0e767e286grg",
    "servicePrincipalDisplayName": "Contoso App",
    "appId": "0grb38ac-a572-491d-a9db-b07197643457",
    "keyIds": [
      "9d9fea30-d8e3-481b-b57c-0ef569a989e5"
    ],
    "additionalInfo": "[{\"Key\":\"alertUrl\",\"Value\":null}]"
    }
  ]
}
```
