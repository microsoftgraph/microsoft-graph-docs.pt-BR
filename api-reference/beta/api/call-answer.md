---
title: 'call: answer'
description: Atenda às chamadas recebidas.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ae80594e940b288403f04aa7885fd5c8e8fb20db
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343208"
---
# <a name="call-answer"></a>call: answer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Habilitar um bot para atender uma [chamada de entrada](../resources/call.md). A solicitação de chamada de entrada pode ser um convite de um participante em uma chamada de grupo ou uma chamada ponto a ponto. Se um convite para uma chamada de grupo for recebido, a notificação conterá os parâmetros [chatInfo](../resources/chatinfo.md) e [meetingInfo](../resources/meetinginfo.md) .

Espera-se que o bot atenda, [rejeite](./call-reject.md) ou [redirecione a](./call-redirect.md) chamada antes do tempo de chamada. O valor de tempo decoro atual é 15 segundos. O valor de tempo decoro atual é de 15 segundos para cenários regulares e 5 segundos para cenários de gravação baseados em política.

## <a name="permissions"></a>Permissões
Você não precisa de nenhuma permissão para responder a uma chamada ponto a ponto. Você precisa de uma das seguintes permissões para ingressar em uma chamada de grupo. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios)                 |
| :-------------- | :-----------------------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Não suportado                        |
| Delegado (conta pessoal da Microsoft) | Não suportado                        |
| Aplicativo     | Calls.JoinGroupCalls.All ou Calls.JoinGroupCallsasGuest.All |

> **Observação:** Para uma chamada que usa mídia hospedada por aplicativo, você também precisa da permissão Calls.AccessMedia.All. `source` Você deve ter pelo menos uma das seguintes permissões para garantir que a notificação de chamada de entrada seja descriptografada: Calls.AccessMedia.All, Calls.Initiate.All, Calls.InitiateGroupCall.All, Calls.JoinGroupCall.All, Calls.JoinGroupCallAsGuest.All. São `source` as informações do chamador na notificação de chamada de entrada. Sem pelo menos uma dessas permissões, o `source` permanecerá criptografado.

## <a name="http-request"></a>Solicitação HTTP
<!-- {"blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /communications/calls/{id}/answer
```
> **Observação:** o caminho `/app` foi preterido. Daqui em diante, use o caminho `/communications`.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |
| Content-type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro           | Tipo                                                                                                                                 | Descrição                                                                                                                                                                                                         |
| :-----------------  | :-----------------------------------------                                                                                           | :----------------------------------------------------------------------------------------------------------------------------------------------                                                                     |
| callbackUri         | String                                                                                                                               | Permite que os bots forneçam um URI de retorno de chamada específico para que a chamada simultânea receba notificações posteriores. Se essa propriedade não tiver sido definida, o URI de retorno de chamada global do bot será usado em vez disso. Isso deve ser `https`. |
| acceptedModalities  | String collection                                                                                                                    | A lista de modalidades de aceitação. Os valores possíveis são: `audio`, `video`, `videoBasedScreenSharing`. Obrigatório para atender uma chamada.                                                                                      |
| mediaConfig         | [appHostedMediaConfig](../resources/apphostedmediaconfig.md) ou [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md) | A configuração de mídia. Necessário.                                                                                                                                                                                 |
| participantCapacity | Int                                                                                                                                  | O número de participantes que o aplicativo pode manipular para a chamada, para Teams [de gravação baseada](/MicrosoftTeams/teams-recording-policy) em política.                                                     |

## <a name="response"></a>Resposta
Este método retorna um código `202 Accepted` de resposta.

## <a name="examples"></a>Exemplos
O exemplo a seguir mostra como chamar essa API.

##### <a name="request"></a>Solicitação
O exemplo a seguir mostra a solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-answer"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/answer
Content-Type: application/json
Content-Length: 211

{
  "callbackUri": "callbackUri-value",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration Blob>"
  },
  "acceptedModalities": [
    "audio"
  ],
  "participantCapacity": 200
}
```
Esse blob é a configuração serializada para sessões de mídia geradas a partir do SDK de mídia.

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/call-answer-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/call-answer-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. 

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a>Exemplo 1: responder a uma chamada VoIP ponto a ponto com mídia hospedada pelo serviço

##### <a name="notification---incoming"></a>Notificação - entrada

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "created",
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
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

<!-- {
  "blockType": "ignored",
  "name": "call-answer-service-hosted-media"
}-->
```http
POST /communications/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Content-Type: application/json

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
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a>Notificação - estabelecimento

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a>Notificação - estabelecida

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
      }
    }
  ]
}
```

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a>Exemplo 2: Atender chamada VOIP com mídia hospedada por aplicativo

##### <a name="notification---incoming"></a>Notificação - entrada

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "created",
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
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
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
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


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-answer-app-hosted-media"
}-->
```http
POST /communications/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Content-Type: application/json

{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration Blob>"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/call-answer-app-hosted-media-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/call-answer-app-hosted-media-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a>Notificação - estabelecimento

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a>Notificação - estabelecida

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
      }
    }
  ]
}
```

### <a name="example-3-answer-a-policy-based-recording-call"></a>Exemplo 3: atender a uma chamada de gravação baseada em política

No cenário [de registro baseado](/microsoftteams/teams-recording-policy) em política, antes de um participante em política ingressar em uma chamada, uma notificação de chamada de entrada será enviada para o bot associado à política.
As informações de junção podem ser encontradas na **propriedade botData** . Em seguida, o bot pode optar por atender à chamada e [atualizar o status da](call-updaterecordingstatus.md) gravação de acordo.

Quando for especificado na solicitação de uma notificação de registro baseada em política, o evento de participação do participante subsequente pertencente ao mesmo grupo de política será enviado como [participanteJoiningNotification](../resources/participantJoiningNotification.md) em vez de uma nova notificação de chamada de entrada, até que o número de participantes que a instância de chamada atual está manipulando tenha atingido o número especificado em `participantCapacity`.`participantCpapacity` `Answer`

Veja a seguir um exemplo da notificação de chamada de entrada que um bot receberia nesse caso.

```json
{
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[
      {
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"created",
         "resource":"/app/calls/e71f0300-9c1f-4d99-b5f4-2722e877d497",
         "resourceUrl":"/communications/calls/e71f0300-9c1f-4d99-b5f4-2722e877d497",
         "resourceData":{
            "@odata.type":"#microsoft.graph.call",
            "state":"incoming",
            "direction":"incoming",
            "source":{
               "@odata.type":"#microsoft.graph.participantInfo",
               "id":"90fad2ce-8989-41a1-8a66-f6636e629a2a",
               "identity":{
                  "@odata.type":"#microsoft.graph.identitySet",
                  "user":{
                     "@odata.type":"#microsoft.graph.identity",
                     "id":"8A34A46B-3D17-4ADC-8DCE-DC4E7D572698",
                     "identityProvider":"AAD"
                  }
               },
               "endpointType":"default",
               "region":"amer"
            },
            "targets":[
               {
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "applicationInstance":{
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"832899f8-2ea1-4604-8413-27bd2892079f",
                        "identityProvider":"AAD"
                     }
                  },
                  "endpointType":"default",
                  "id":"4520a1a5-5394-5a41-aa12-9ee6fa18cfc8",
                  "region":null,
                  "languageId":null
               }
            ],
            "meetingInfo":{
               "@odata.type":"#microsoft.graph.tokenMeetingInfo",
               "token":"join token"
            },
            "tenantId":"932899f8-2ea1-4604-8413-27bd2892079f",
            "myParticipantId":"1520a1a5-5394-4a41-aa72-9ee6fa18cfc8",
            "callChainId":"05f2f70f-3a9c-47c1-80a9-cc79e91d8cec",
            "incomingContext":{
               "@odata.type":"#microsoft.graph.incomingContext",
               "sourceParticipantId":"30fad2ce-8989-41a1-8a66-f6636e629a2a",
               "observedParticipantId":"30fad2ce-8989-41a1-8a66-f6636e629a2a"
            },
            "id":"e71f0300-9c1f-4d99-b5f4-2722e877d497",
            "applicationMetadata":{
               "botData":{
                  "mediaHostedRegion":"USEA",
                  "user":{
                     "participationMethod":"callee",
                     "clientLocation":"US"
                  },
                  "otherSideUser":{
                     "id":"971f0300-9c1f-4d99-b5f4-2722e877d490",
                     "participantId":"3520a1a5-5394-4a41-aa72-9ee6fa18cfc8",
                     "tenantId":"1540a1a5-2394-4a41-aa72-9ee6fa18cfc8",
                     "onBehalfOf":{
                        "id":"871f0300-9c1f-4d99-b5f4-2722e877d490"
                     },
                     "participationMethod":"caller",
                     "clientLocation":"EUNO"
                  },
                  "inviteReasons":[
                     "PolicyBasedRecording"
                  ],
                  "policyIdentifier":"Test Policy",
                  "pairedRecorders":[
                     {
                        "id":"471f0300-5c1f-4d99-b5f4-2722e877d490",
                        "participantId":"371f0300-2c1f-4d99-b5f4-2722e877d490"
                     }
                  ],
                  "otherRecorders":[
                     {
                        "id":"671f0300-9c1f-4d99-b5f4-2722e877d490",
                        "participantId":"a71f0300-ec1f-4d99-b5f4-2722e877d490"
                     }
                  ]
               }
            }
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
  ]
}
-->
