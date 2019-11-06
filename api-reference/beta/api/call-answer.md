---
title: 'Call: resposta'
description: Atenda às chamadas recebidas.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 5c9b506b8fc10bcec48e503e394b813e79f8ad82
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006365"
---
# <a name="call-answer"></a><span data-ttu-id="e5b60-103">Call: resposta</span><span class="sxs-lookup"><span data-stu-id="e5b60-103">call: answer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5b60-104">Habilite um bot para atender a uma [chamada](../resources/call.md)de entrada.</span><span class="sxs-lookup"><span data-stu-id="e5b60-104">Enable a bot to answer an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="e5b60-105">A solicitação de chamada de entrada pode ser um convite de um participante em uma chamada de grupo ou uma chamada ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="e5b60-105">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="e5b60-106">Se for recebido um convite para uma chamada de grupo, a notificação conterá os parâmetros [chatInfo](../resources/chatinfo.md) e [meetingInfo](../resources/meetinginfo.md) .</span><span class="sxs-lookup"><span data-stu-id="e5b60-106">If an invite to a group call is received, the notification will contain the [chatInfo](../resources/chatinfo.md) and [meetingInfo](../resources/meetinginfo.md) parameters.</span></span>

<span data-ttu-id="e5b60-107">O bot deve responder ou [rejeitar](./call-reject.md) a chamada antes do tempo limite da chamada. O valor de tempo limite atual é de 15 segundos.</span><span class="sxs-lookup"><span data-stu-id="e5b60-107">The bot is expected to answer or [reject](./call-reject.md) the call before the call times out. The current timeout value is 15 seconds.</span></span>

> <span data-ttu-id="e5b60-108">**Observação:** O bot só pode ser acessado por VoIP.</span><span class="sxs-lookup"><span data-stu-id="e5b60-108">**Note:** The bot can only be reached by VoIP.</span></span> <span data-ttu-id="e5b60-109">Não há suporte para a chamada PSTN.</span><span class="sxs-lookup"><span data-stu-id="e5b60-109">PSTN calling isn't supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5b60-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="e5b60-110">Permissions</span></span>
<span data-ttu-id="e5b60-111">Você não precisa de nenhuma permissão para responder a uma chamada ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="e5b60-111">You do not need any permissions to answer a peer-to-peer call.</span></span> <span data-ttu-id="e5b60-112">Você precisa de uma das seguintes permissões para ingressar em uma chamada de grupo.</span><span class="sxs-lookup"><span data-stu-id="e5b60-112">You need one of the following permissions to join a group call.</span></span> <span data-ttu-id="e5b60-113">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5b60-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5b60-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5b60-114">Permission type</span></span> | <span data-ttu-id="e5b60-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5b60-115">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="e5b60-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5b60-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5b60-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="e5b60-117">Not Supported</span></span>                        |
| <span data-ttu-id="e5b60-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5b60-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5b60-119">Não suportado</span><span class="sxs-lookup"><span data-stu-id="e5b60-119">Not Supported</span></span>                        |
| <span data-ttu-id="e5b60-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5b60-120">Application</span></span>     | <span data-ttu-id="e5b60-121">Calls. JoinGroupCalls. All ou calls. JoinGroupCallsasGuest. All</span><span class="sxs-lookup"><span data-stu-id="e5b60-121">Calls.JoinGroupCalls.All or Calls.JoinGroupCallsasGuest.All</span></span>                                                         |

> <span data-ttu-id="e5b60-122">**Observação:** Para uma chamada que usa mídia hospedada por aplicativo, você também precisa da permissão calls. AccessMedia. All.</span><span class="sxs-lookup"><span data-stu-id="e5b60-122">**Note:** For a call that uses application-hosted media, you also need the Calls.AccessMedia.All permission.</span></span>                                                   |

## <a name="http-request"></a><span data-ttu-id="e5b60-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5b60-123">HTTP request</span></span>
<!-- {"blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /communications/calls/{id}/answer
```
> <span data-ttu-id="e5b60-124">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="e5b60-124">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="e5b60-125">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="e5b60-125">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5b60-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5b60-126">Request headers</span></span>
| <span data-ttu-id="e5b60-127">Nome</span><span class="sxs-lookup"><span data-stu-id="e5b60-127">Name</span></span>          | <span data-ttu-id="e5b60-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5b60-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e5b60-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5b60-129">Authorization</span></span> | <span data-ttu-id="e5b60-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5b60-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5b60-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="e5b60-132">Content-type</span></span>  | <span data-ttu-id="e5b60-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5b60-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5b60-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5b60-135">Request body</span></span>
<span data-ttu-id="e5b60-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5b60-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e5b60-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e5b60-137">Parameter</span></span>        | <span data-ttu-id="e5b60-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5b60-138">Type</span></span>                                     |<span data-ttu-id="e5b60-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5b60-139">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="e5b60-140">callbackUri</span><span class="sxs-lookup"><span data-stu-id="e5b60-140">callbackUri</span></span>       |<span data-ttu-id="e5b60-141">String</span><span class="sxs-lookup"><span data-stu-id="e5b60-141">String</span></span>                                    |<span data-ttu-id="e5b60-142">Isso permite que os bots forneçam um URI de retorno de chamada específico para que a chamada atual receba notificações posteriores.</span><span class="sxs-lookup"><span data-stu-id="e5b60-142">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="e5b60-143">Se essa propriedade não tiver sido definida, o URI de retorno de chamada global do bot será usado em seu lugar.</span><span class="sxs-lookup"><span data-stu-id="e5b60-143">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="e5b60-144">Deve ser `https`.</span><span class="sxs-lookup"><span data-stu-id="e5b60-144">This must be `https`.</span></span>    |
|<span data-ttu-id="e5b60-145">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="e5b60-145">acceptedModalities</span></span>|<span data-ttu-id="e5b60-146">String collection</span><span class="sxs-lookup"><span data-stu-id="e5b60-146">String collection</span></span>                         |<span data-ttu-id="e5b60-147">A lista de aceitar modalidades.</span><span class="sxs-lookup"><span data-stu-id="e5b60-147">The list of accept modalities.</span></span> <span data-ttu-id="e5b60-148">O valor possível são `audio`: `video`, `videoBasedScreenSharing`,.</span><span class="sxs-lookup"><span data-stu-id="e5b60-148">Possible value are: `audio`, `video`, `videoBasedScreenSharing`.</span></span> <span data-ttu-id="e5b60-149">Obrigatório para responder a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="e5b60-149">Required for answering a call.</span></span> |
|<span data-ttu-id="e5b60-150">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="e5b60-150">mediaConfig</span></span>       | <span data-ttu-id="e5b60-151">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) ou [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="e5b60-151">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) or [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span></span> |<span data-ttu-id="e5b60-152">A configuração de mídia.</span><span class="sxs-lookup"><span data-stu-id="e5b60-152">The media configuration.</span></span> <span data-ttu-id="e5b60-153">Precisam</span><span class="sxs-lookup"><span data-stu-id="e5b60-153">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="e5b60-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5b60-154">Response</span></span>
<span data-ttu-id="e5b60-155">Este método retorna `202 Accepted` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5b60-155">This method returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e5b60-156">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e5b60-156">Examples</span></span>
<span data-ttu-id="e5b60-157">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e5b60-157">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e5b60-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5b60-158">Request</span></span>
<span data-ttu-id="e5b60-159">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5b60-159">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e5b60-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5b60-160">HTTP</span></span>](#tab/http)
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
  ]
}
```
<span data-ttu-id="e5b60-161">Este blob é a configuração serializada para sessões de mídia que é gerada a partir do SDK de mídia.</span><span class="sxs-lookup"><span data-stu-id="e5b60-161">This blob is the serialized configuration for media sessions which is generated from the media SDK.</span></span>

# <a name="ctabcsharp"></a>[<span data-ttu-id="e5b60-162">C#</span><span class="sxs-lookup"><span data-stu-id="e5b60-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e5b60-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5b60-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e5b60-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5b60-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e5b60-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5b60-165">Response</span></span>
<span data-ttu-id="e5b60-166">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5b60-166">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="e5b60-167">Exemplo 1: responder a uma chamada VoIP ponto a ponto com mídia hospedada no serviço</span><span class="sxs-lookup"><span data-stu-id="e5b60-167">Example 1: Answer a Peer-to-Peer VoIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="e5b60-168">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="e5b60-168">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="e5b60-169">Solicitar</span><span class="sxs-lookup"><span data-stu-id="e5b60-169">Request</span></span>

<!-- {
  "blockType": "request",
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

##### <a name="response"></a><span data-ttu-id="e5b60-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5b60-170">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="e5b60-171">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="e5b60-171">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="e5b60-172">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="e5b60-172">Notification - established</span></span>

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

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="e5b60-173">Exemplo 2: responder a chamada VOIP com mídia hospedada por aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5b60-173">Example 2: Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="e5b60-174">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="e5b60-174">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="e5b60-175">Solicitar</span><span class="sxs-lookup"><span data-stu-id="e5b60-175">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="e5b60-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5b60-176">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="e5b60-177">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="e5b60-177">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="e5b60-178">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="e5b60-178">Notification - established</span></span>

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
