---
title: Obter trabalho em equipeDevice
description: Obter as propriedades de um dispositivo Microsoft Teams habilitado para uso, incluindo tipo de dispositivo, detalhes de hardware, estado de atividade e informações de status de saúde.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 2c77cf72923593ef42f36280046809453c20f305
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262292"
---
# <a name="get-teamworkdevice"></a>Obter trabalho em equipeDevice
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter as propriedades de um Microsoft Teams habilitado para [Microsoft Teams.](../resources/teamworkdevice.md) Por exemplo, você pode usar esse método para obter o tipo de dispositivo, detalhes de hardware, estado de atividade e informações de status de saúde para um dispositivo habilitado para Teams.

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
GET /teamwork/devices/{teamworkDeviceId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Essa operação dá suporte ao parâmetro `$select` [de consulta OData](/graph/query-parameters) para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [teamworkDevice](../resources/teamworkdevice.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "get_teamworkdevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkDevice"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamworkDevice",
    "id": "0f3ce432-e432-0f3c-32e4-3c0f32e43c0f",
    "deviceType": "CollaborationBar",
    "hardwareDetail": {
      "serialNumber": "0189",
      "uniqueId": "5abcdefgh",
      "macAddresses": [],
      "manufacturer": "yealink",
      "model": "vc210"
    },
    "notes": "CollaborationBar device.",
    "companyAssetTag": "Tag1",
    "healthStatus": "Healthy",
    "activityState": "Idle",
    "createdDateTime": "2021-06-19T19:01:04.185Z",
    "createdBy": null,
    "lastModifiedDateTime": "2021-06-19T19:01:04.185Z",
    "lastModifiedBy": null,
    "currentUser": {
      "id": "2a610f6f-adf6-4205",
      "displayName": "Evan Lewis",
      "userIdentityType": "aadUser"
    }
  }
}
```

