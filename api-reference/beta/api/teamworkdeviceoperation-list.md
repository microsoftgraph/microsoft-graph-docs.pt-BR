---
title: Listar trabalho em equipeDeviceOperations
description: Obter uma lista de operações vinculadas a um dispositivo Microsoft Teams habilitado para Microsoft Teams.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 50ef765c313bf1e0508509cbc41f3b2453cbf5b0
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262296"
---
# <a name="list-teamworkdeviceoperations"></a>Listar trabalho em equipeDeviceOperations
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista das [operações que](../resources/teamworkdeviceoperation.md) estão sendo executados em um dispositivo Microsoft Teams habilitado para [uso.](../resources/teamworkdevice.md)

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
GET /teamwork/devices/{teamworkDeviceId}/operations
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método suporta o `$top`, `$select`, e `$skipToken` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

### <a name="supported-query-patterns"></a>Padrões de consulta com suporte

| Padrão                | Sintaxe                                 | Observações |
| ---------------------- | -------------------------------------- | ----- |
| Paginação do lado do servidor | `@odata.nextLink`                      | Você receberá um token de continuação na resposta, quando um conjunto de resultados abrange várias páginas. |
| Limite de página                 | `/devices({deviceId})/operations?$top=10` | Obter operações para um dispositivo com um tamanho de página de 10. O limite padrão da página é 20. O limite máximo da página é 50. |

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [teamworkDeviceOperation](../resources/teamworkdeviceoperation.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_teamworkdeviceoperation"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f/operations
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkDeviceOperation",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teamwork/devices('18129e1f')/operations",
  "@odata.count": 1,
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamworkDeviceOperation",
      "id": "eab261f8-61f8-eab2-f861-b2eaf861b2ea",
      "status": "successful",
      "operationType": "deviceDiagnostics",
      "error": {
        "code": null,
        "message": "Unknown"
      },
      "startedDateTime": "2021-06-19T12-01-03.45Z",
      "completedDateTime": "2021-06-19T12-01-03.45Z",
      "createdDateTime": "2021-06-19T12-01-03.45Z",
      "lastActionDateTime": "2021-06-19T12-01-03.45Z",
      "createdBy": {
        "application": null,
        "device": null,
        "user": {
          "id": "2a610f6f-adf6-4205",
          "displayName": "Evan Lewis",
          "userIdentityType": "aadUser"
        }
      },
      "lastActionBy": {
        "application": null,
        "device": null,
        "user": {
          "id": "2a610f6f-adf6-4205",
          "displayName": "Evan Lewis",
          "userIdentityType": "aadUser"
        }
      }
    }
  ]
}
```

