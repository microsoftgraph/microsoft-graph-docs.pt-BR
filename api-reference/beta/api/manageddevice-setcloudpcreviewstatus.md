---
title: 'managedDevice: setCloudPcReviewStatus'
description: Defina o status de revisão de um dispositivo de PC na nuvem específico.
author: yayang3
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 3b894035944f2a2962d9b28ceb7e72012ccd5ac7
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629487"
---
# <a name="manageddevice-setcloudpcreviewstatus"></a>managedDevice: setCloudPcReviewStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Defina o status de revisão de um dispositivo de PC na nuvem específico. Use essa API para definir o status de revisão de um PC na nuvem para revisão se você considerar um PC na nuvem suspeito. Depois que a revisão for concluída, use essa API novamente para definir o PC na nuvem de volta para um estado normal.

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
POST /deviceManagement/managedDevices/{managedDeviceId}/setCloudPcReviewStatus
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra o parâmetro que pode ser usado com essa ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|reviewStatus|[cloudPcReviewStatus](../resources/cloudpcreviewstatus.md)|O novo status de revisão do PC na nuvem.|


## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "request",
  "name": "manageddevicethis.setcloudpcreviewstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/185f01c2de954929afb129392e5d9f47/setCloudPcReviewStatus
Content-Type: application/json

{
  "reviewStatus": {
    "inReview": true,
    "userAccessLevel": "restricted",
    "azureStorageAccountId": "/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview"
  }
}
```


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "manageddevicethis.setcloudpcreviewstatus"
}
-->
``` http
HTTP/1.1 204 No Content
```

