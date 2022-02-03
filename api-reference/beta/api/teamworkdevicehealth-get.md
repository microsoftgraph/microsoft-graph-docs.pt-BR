---
title: Obter trabalho em equipeDeviceHealth
description: Obter os detalhes de saúde de um Microsoft Teams habilitado para uso.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: acf9d7d8b0f2628739debd1ce97421e8e8a4b18a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349011"
---
# <a name="get-teamworkdevicehealth"></a>Obter trabalho em equipeDeviceHealth
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter os [detalhes de](../resources/teamworkdevicehealth.md) saúde de um dispositivo Microsoft Teams [habilitado para uso.](../resources/teamworkdevice.md) A saúde do dispositivo é calculada com base na configuração do dispositivo e em outros parâmetros de dispositivo.

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
GET /teamwork/devices/{teamworkDeviceId}/health
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

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [teamworkDeviceHealth](../resources/teamworkdevicehealth.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamworkdevicehealth"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/devices/d8214fe3-4fe3-d821-e34f-21d8e34f21d8/health
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamworkdevicehealth-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamworkdevicehealth-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamworkdevicehealth-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamworkdevicehealth-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-teamworkdevicehealth-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-teamworkdevicehealth-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkDeviceHealth"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamworkDeviceHealth",
    "id": "d8214fe3-4fe3-d821-e34f-21d8e34f21d8",
    "connection": {
      "connectionStatus": "disconnected",
      "lastModifiedDateTime": "2021-06-10T19:01:04.185Z"
    },
    "loginStatus": {
      "exchangeConnection": {
        "connectionStatus": "connected",
        "lastModifiedDateTime": "2021-06-10T19:01:04.185Z"
      },
      "teamsConnection": {
        "connectionStatus": "connected",
        "lastModifiedDateTime": "2021-06-10T19:01:04.185Z"
      },
      "skypeConnection": {
        "connectionStatus": "connected",
        "lastModifiedDateTime": "2021-06-10T19:01:04.185Z"
      }
    },
    "peripheralsHealth": {
      "roomCameraHealth": {
        "isOptional": false,
        "connection": {
          "connectionStatus": "disconnected",
          "lastModifiedDateTime": "2021-06-10T19:01:04.185Z"
        }
      },
      "contentCameraHealth": {
        "isOptional": true,
        "connection": {
          "connectionStatus": "unknown",
          "lastModifiedDateTime": "2021-06-10T19:01:04.185Z"
        }
      },
      "speakerHealth": {
        "isOptional": false,
        "connection": {
          "connectionStatus": "connected",
          "lastModifiedDateTime": "2021-06-10T19:01:04.185Z"
        }
      },
      "communicationSpeakerHealth": {
        "isOptional": false,
        "connection": {
          "connectionStatus": "connected",
          "lastModifiedDateTime": "2021-06-10T19:01:04.185Z"
        }
      },
      "displayHealthCollection": [
          {
            "isOptional": false,
            "connection": {
              "connectionStatus": "disconnected",
              "lastModifiedDateTime": "2021-06-10T19:01:04.185Z"
            }
          },
          {
            "isOptional": true,
            "connection": {
              "connectionStatus": "disconnected",
              "lastModifiedDateTime": "2021-06-10T19:01:04.185Z"
            }
          }
      ],
      "microphoneHealth": {
        "isOptional": false,
        "connection": {
          "connectionStatus": "connected",
          "lastModifiedDateTime": "2021-06-10T19:01:04.185Z"
        }
      }
    },
    "softwareUpdateHealth": {
      "companyPortalSoftwareUpdateStatus": null,
      "firmwareSoftwareUpdateStatus": null,
      "partnerAgentSoftwareUpdateStatus": null,
      "adminAgentSoftwareUpdateStatus": {
          "softwareFreshness": "latest",
          "currentVersion": "2021.4.4.8",
          "availableVersion": null
      },
      "teamsClientSoftwareUpdateStatus": null,
      "operatingSystemSoftwareUpdateStatus": null
    },
    "hardwareHealth": {
      "computeHealth": {
        "isOptional": false,
        "connection": {
            "connectionStatus": "connected",
            "lastModifiedDateTime": "2021-06-10T19:01:04.185Z"
        }
      },
      "hdmiIngestHealth": {
        "isOptional": false,
        "connection": {
            "connectionStatus": "connected",
            "lastModifiedDateTime": "2021-06-10T19:01:04.185Z"
        }
      }
    },
    "createdDateTime": "2021-03-19T19:00:04.000Z",
    "lastModifiedDateTime": "2021-06-19T19:01:04.185Z",
    "createdBy": null,
    "lastModifiedBy": null
  }
}
```

