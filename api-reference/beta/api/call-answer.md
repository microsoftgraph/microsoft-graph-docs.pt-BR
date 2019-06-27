---
title: 'Call: resposta'
description: Atenda às chamadas recebidas.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b938bde443f59612b3376595e06ed22041d470c0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262357"
---
# <a name="call-answer"></a>Call: resposta

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atenda às chamadas recebidas.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios)                 |
| :-------------- | :-----------------------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Não suportado                        |
| Delegado (conta pessoal da Microsoft) | Não suportado                        |
| Aplicativo     | Nenhum                                                        |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /applications/{id}/calls/{id}/answer
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro        | Tipo                                     |Descrição                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|callbackUri       |String                                    |A ID de retorno de chamada ou de assinatura à qual os retornos serão entregues. Precisam                                                               |
|acceptedModalities|Coleção de cadeias de caracteres                         |A lista de aceitar modalidades. O valor possível são `unknown`: `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`,. Precisam |
|mediaConfig       |[mediaConfig](../resources/mediaconfig.md)|A configuração de mídia. Precisam                                                                                                            |

## <a name="response"></a>Resposta
Este método retorna `202 Accepted` um código de resposta.

## <a name="examples"></a>Exemplos
O exemplo a seguir mostra como chamar essa API.

##### <a name="request"></a>Solicitação
O exemplo a seguir mostra a solicitação.

<!-- {
  "blockType": "request",
  "name": "call-answer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/answer
Content-Type: application/json
Content-Length: 211

{
  "callbackUri": "callbackUri-value",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  },
  "acceptedModalities": [
    "audio"
  ]
}
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/call-answer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-answer-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/call-answer-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="answer-voip-call-with-service-hosted-media"></a>Responder chamada VOIP com mídia hospedada pelo serviço

##### <a name="notification---incoming"></a>Notificação-entrada

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "callRoutes": [
          {
            "routingType": "lookup",
            "original": {
              "phone": {
                "id": "+14258828080"
              }
            },
            "final": {
              "user": {
                "id": "29362BD4-CD58-4ED0-A206-0E4A33DBB0B6",
                "displayName": "Heidi Steen"
              }
            }
          }
        ],
        "source": {
          "identity": {
            "user": {
              "displayName": "Test User",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a>Solicitação

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "ignored",
  "name": "call-answer"
}-->
```json
{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
      {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        "uri": "https://cdn.contoso.com/cool.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  }
}
```

##### <a name="response"></a>Resposta

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a>Notificação-estabelecimento

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a>Estabelecido em notificação

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
      }
    }
  ]
}
```

### <a name="answer-voip-call-with-application-hosted-media"></a>Responder chamada VOIP com mídia hospedada por aplicativo

##### <a name="notification---incoming"></a>Notificação-entrada

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "user": {
              "displayName": "Test User",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a>Solicitação

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "ignored",
  "name": "call-answer"
}-->
```json
{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  }
}
```

##### <a name="response"></a>Resposta

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a>Notificação-estabelecimento

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a>Estabelecido em notificação

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: answer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-answer.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/call-answer.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-answer.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
