---
title: Obter trabalho em equipeDeviceActivity
description: Obter o status de atividade de um dispositivo Microsoft Teams habilitado para uso.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: cd55e6e939aa96c2ce879b657fcf4ebe9e38b196
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262303"
---
# <a name="get-teamworkdeviceactivity"></a>Obter trabalho em equipeDeviceActivity
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter o [status de](../resources/teamworkdeviceactivity.md) atividade de um dispositivo Microsoft Teams [habilitado para uso.](../resources/teamworkdevice.md) 

[!INCLUDE [teamworkdevice-api-disclaimer](../../includes/teamworkdevice-api-disclaimer.md)]

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|TeamworkDevice.Read.All, TeamworkDevice.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|TeamworkDevice.Read.All, TeamworkDevice.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teamwork/devices/{teamworkDeviceId}/activity
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esta operação dá suporte aos parâmetros `$select` `$expand` [de consulta e OData](/graph/query-parameters) para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [teamworkDeviceActivity](../resources/teamworkdeviceactivity.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "get_teamworkdeviceactivity"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/devices/1ae3fe60-fe60-1ae3-60fe-e31a60fee31a/activity
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkDeviceActivity"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamworkDeviceActivity",
    "id": "1ae3fe60-fe60-1ae3-60fe-e31a60fee31a",
    "activePeripherals": {
      "roomCamera": null,
      "contentCamera": null,
      "speaker": {
        "id": "Headset Earphone (Logitech SmartDock)",
        "displayName": "Headset Earphone (Logitech SmartDock)",
        "vendorId": "VID_046D",
        "productId": "PID_0864"
      },
      "communicationSpeaker": {
        "id": "Headset Earphone (Logitech SmartDock)",
        "displayName": "Headset Earphone (Logitech SmartDock)",
        "vendorId": "VID_046D",
        "productId": "PID_0864"
      },
      "microphone": {
        "id": "Headset Microphone (Logitech SmartDock)",
        "displayName": "Headset Microphone (Logitech SmartDock)",
        "vendorId": "VID_046D",
        "productId": "PID_0864"
      },
    },
    "createdDateTime": "2021-03-19T19:00:04.000Z",
    "lastModifiedDateTime": "2021-06-19T19:01:04.185Z",
    "createdBy": null,
    "lastModifiedBy": null
  }
}
```

