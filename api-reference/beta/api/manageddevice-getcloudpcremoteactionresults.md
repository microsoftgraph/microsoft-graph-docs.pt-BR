---
title: 'managedDevice: getCloudPcRemoteActionResults'
description: Verifique o status de ação remota especificada pelo computador na nuvem para um dispositivo cloud pc.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: cd47cf2c04bad5ffc0428516182829aa7ecb0ebf
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766783"
---
# <a name="manageddevice-getcloudpcremoteactionresults"></a>managedDevice: getCloudPcRemoteActionResults

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Verifique os resultados da ação remota especificada pelo [computador na nuvem](../resources/cloudpcremoteactionresult.md) para um dispositivo cloud pc. O Cloud PC dá suporte a reprovisionamento e ressarmos ações remotas.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|CloudPC.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/managedDevices/{managedDeviceId}/getCloudPcRemoteActionResults
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "managedDevice_getCloudPcRemoteActionResults"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/getCloudPcRemoteActionResults
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/manageddevice-getcloudpcremoteactionresults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/manageddevice-getcloudpcremoteactionresults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/manageddevice-getcloudpcremoteactionresults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/manageddevice-getcloudpcremoteactionresults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcRemoteActionResult"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.cloudPcRemoteActionResult)",
    "value": [{
        "actionName": "Reprovision",
        "actionState": "pending",
        "startDateTime": "2021-04-25T02:04:53.4722004Z",
        "lastUpdatedDateTime": "2021-04-25T02:04:53.4722016Z",
        "cloudPcId": "96b3203b-9dc2-48cb-b1e3-a80822ffffff",
        "managedDeviceId": "8e1a54a7-33f6-4659-86b7-dde7c2ffffff",
        "statusDetails": null
    }]
}
```
