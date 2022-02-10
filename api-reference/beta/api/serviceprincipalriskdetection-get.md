---
title: Obter servicePrincipalRiskDetection
description: Leia as propriedades e as relações de um objeto servicePrincipalRiskDetection.
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a8eb1fe358b0e9a250fa16754ef0b9e5a413a2a5
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519945"
---
# <a name="get-serviceprincipalriskdetection"></a>Obter servicePrincipalRiskDetection
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto servicePrincipalRiskDetection](../resources/serviceprincipalriskdetection.md) .

>**Observação:** Você deve ter uma Azure AD Premium P1 ou P2 para usar a API servicePrincipalRiskDetection.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|IdentityRiskyServicePrincipal.Read.All, IdentityRiskyServicePrincipal.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|IdentityRiskyServicePrincipal.Read.All, IdentityRiskyServicePrincipal.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/servicePrincipalRiskDetections/{servicePrincipalRiskDetectionId}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um [objeto servicePrincipalRiskDetection](../resources/serviceprincipalriskdetection.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-a-specific-risk-detection-object"></a>Exemplo 1: Obter um objeto de detecção de risco específico

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipalriskdetection"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityProtection/servicePrincipalRiskDetections/{servicePrincipalRiskDetectionId}
```


#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipalRiskDetection"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
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
}
```

