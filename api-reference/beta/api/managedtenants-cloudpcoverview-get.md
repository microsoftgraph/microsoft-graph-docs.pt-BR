---
title: Obter cloudPcOverview
description: Leia as propriedades e as relações de um objeto cloudPcOverview.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 6bae6f583b793dc5d1b94ad368708137ae18805d
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440068"
---
# <a name="get-cloudpcoverview"></a>Obter cloudPcOverview
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto cloudPcOverview.](../resources/managedtenants-cloudpcoverview.md)

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|CloudPC.Read.All, CloudPC.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcsOverview/{cloudPcOverviewId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcoverview"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcsOverview/{cloudPcOverviewId}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcoverview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcoverview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcoverview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcoverview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.cloudPcOverview"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcOverview",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "tenantDisplayName": "Fourth Coffee",
  "totalCloudPcStatus": 18,
  "numberOfCloudPcStatusNotProvisioned": 4,
  "numberOfCloudPcStatusProvisioning": 0,
  "numberOfCloudPcStatusProvisioned": 14,
  "numberOfCloudPcStatusUpgrading": 0,
  "numberOfCloudPcStatusInGracePeriod": 0,
  "numberOfCloudPcStatusDeprovisioning": 0,
  "numberOfCloudPcStatusFailed": 0,
  "numberOfCloudPcStatusUnknown": 0,
  "totalCloudPcConnectionStatus": 25,
  "numberOfCloudPcConnectionStatusPending": 0,
  "numberOfCloudPcConnectionStatusRunning": 0,
  "numberOfCloudPcConnectionStatusPassed": 17,
  "numberOfCloudPcConnectionStatusFailed": 6,
  "numberOfCloudPcConnectionStatusUnkownFutureValue": 0,
  "lastRefreshedDateTime": "2021-07-11T17:18:46.4830816Z"
}
```
