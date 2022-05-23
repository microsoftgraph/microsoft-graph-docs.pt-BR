---
title: 'managedDevice: getCloudPcReviewStatus'
description: Obter o status de revisão de um dispositivo de PC na nuvem específico.
author: yayang3
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: e238118d0bdbbc0bc3990fea33479e01d144c61a
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629488"
---
# <a name="manageddevice-getcloudpcreviewstatus"></a>managedDevice: getCloudPcReviewStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter o status de revisão de um dispositivo de PC na nuvem específico.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC.Read.All, CloudPC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|CloudPC.Read.All, CloudPC.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices/{managedDeviceId}/getCloudPcReviewStatus
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará um código `200 OK` de resposta e um objeto [cloudPcReviewStatus](../resources/cloudpcreviewstatus.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "request",
  "name": "manageddevicethis.getcloudpcreviewstatus"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices/185f01c2de954929afb129392e5d9f47/getCloudPcReviewStatus
```


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.cloudPcReviewStatus",
  "name": "manageddevicethis.getcloudpcreviewstatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "microsoft.graph.cloudPcReviewStatus",
    "inReview": true,
    "userAccessLevel": "restricted",
    "reviewStartDateTime": "2022-02-15T06:52:34Z",
    "restorePointDateTime": "2022-02-15T07:05:03Z",
    "subscriptionId": "f68bd846-16ad-4b51-a7c6-c84944a3367c",
    "subscriptionName": "deschutes-INT-DR-test",
    "azureStorageAccountId": "/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview",
    "azureStorageAccountName": "snapshotsUnderReview"
}
```

