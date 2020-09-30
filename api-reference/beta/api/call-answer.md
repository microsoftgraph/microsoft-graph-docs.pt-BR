---
title: 'Call: resposta'
description: Atenda às chamadas recebidas.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 4182c743859d9ec4bf23a3cf0a86b99662060de8
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313090"
---
# <a name="call-answer"></a><span data-ttu-id="94fda-103">Call: resposta</span><span class="sxs-lookup"><span data-stu-id="94fda-103">call: answer</span></span>

<span data-ttu-id="94fda-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94fda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94fda-105">Habilite um bot para atender a uma [chamada](../resources/call.md)de entrada.</span><span class="sxs-lookup"><span data-stu-id="94fda-105">Enable a bot to answer an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="94fda-106">A solicitação de chamada de entrada pode ser um convite de um participante em uma chamada de grupo ou uma chamada ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="94fda-106">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="94fda-107">Se for recebido um convite para uma chamada de grupo, a notificação conterá os parâmetros [chatInfo](../resources/chatinfo.md) e [meetingInfo](../resources/meetinginfo.md) .</span><span class="sxs-lookup"><span data-stu-id="94fda-107">If an invite to a group call is received, the notification will contain the [chatInfo](../resources/chatinfo.md) and [meetingInfo](../resources/meetinginfo.md) parameters.</span></span>

<span data-ttu-id="94fda-108">O bot deve responder, [rejeitar](./call-reject.md) ou [redirecionar](./call-redirect.md) a chamada antes que a chamada expire. O valor de tempo limite atual é de 15 segundos.</span><span class="sxs-lookup"><span data-stu-id="94fda-108">The bot is expected to answer, [reject](./call-reject.md) or [redirect](./call-redirect.md) the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="94fda-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="94fda-109">Permissions</span></span>
<span data-ttu-id="94fda-110">Você não precisa de nenhuma permissão para responder a uma chamada ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="94fda-110">You do not need any permissions to answer a peer-to-peer call.</span></span> <span data-ttu-id="94fda-111">Você precisa de uma das seguintes permissões para ingressar em uma chamada de grupo.</span><span class="sxs-lookup"><span data-stu-id="94fda-111">You need one of the following permissions to join a group call.</span></span> <span data-ttu-id="94fda-112">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94fda-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94fda-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94fda-113">Permission type</span></span> | <span data-ttu-id="94fda-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94fda-114">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="94fda-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94fda-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="94fda-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="94fda-116">Not Supported</span></span>                        |
| <span data-ttu-id="94fda-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94fda-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94fda-118">Não suportado</span><span class="sxs-lookup"><span data-stu-id="94fda-118">Not Supported</span></span>                        |
| <span data-ttu-id="94fda-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94fda-119">Application</span></span>     | <span data-ttu-id="94fda-120">Calls. JoinGroupCalls. All ou calls. JoinGroupCallsasGuest. All</span><span class="sxs-lookup"><span data-stu-id="94fda-120">Calls.JoinGroupCalls.All or Calls.JoinGroupCallsasGuest.All</span></span> |

> <span data-ttu-id="94fda-121">**Observação:** Para uma chamada que usa mídia hospedada por aplicativo, você também precisa da permissão calls. AccessMedia. All.</span><span class="sxs-lookup"><span data-stu-id="94fda-121">**Note:** For a call that uses application-hosted media, you also need the Calls.AccessMedia.All permission.</span></span> <span data-ttu-id="94fda-122">Você deve ter pelo menos uma das seguintes permissões para garantir que o `source` na notificação de chamada de entrada seja descriptografado: calls. AccessMedia. All, Calls.Initiate. All, Calls.InitiateGroupCall. All, calls. JoinGroupCall. All, calls. JoinGroupCallAsGuest. All.</span><span class="sxs-lookup"><span data-stu-id="94fda-122">You must have at least one of the following permissions to ensure that the `source` in the incoming call notification is decrypted: Calls.AccessMedia.All, Calls.Initiate.All, Calls.InitiateGroupCall.All, Calls.JoinGroupCall.All, Calls.JoinGroupCallAsGuest.All.</span></span> <span data-ttu-id="94fda-123">O `source` é a informação do chamador na notificação de chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="94fda-123">The `source` is the caller info in the incoming call notification.</span></span> <span data-ttu-id="94fda-124">Sem pelo menos uma dessas permissões, o `source` permanecerá criptografado.</span><span class="sxs-lookup"><span data-stu-id="94fda-124">Without at least one of these permissions, the `source` will remain encrypted.</span></span>

## <a name="http-request"></a><span data-ttu-id="94fda-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94fda-125">HTTP request</span></span>
<!-- {"blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /communications/calls/{id}/answer
```
> <span data-ttu-id="94fda-126">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="94fda-126">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="94fda-127">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="94fda-127">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94fda-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94fda-128">Request headers</span></span>
| <span data-ttu-id="94fda-129">Nome</span><span class="sxs-lookup"><span data-stu-id="94fda-129">Name</span></span>          | <span data-ttu-id="94fda-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="94fda-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="94fda-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="94fda-131">Authorization</span></span> | <span data-ttu-id="94fda-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94fda-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94fda-134">Content-type</span><span class="sxs-lookup"><span data-stu-id="94fda-134">Content-type</span></span>  | <span data-ttu-id="94fda-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94fda-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94fda-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94fda-137">Request body</span></span>
<span data-ttu-id="94fda-138">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94fda-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="94fda-139">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="94fda-139">Parameter</span></span>        | <span data-ttu-id="94fda-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="94fda-140">Type</span></span>                                     |<span data-ttu-id="94fda-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="94fda-141">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="94fda-142">callbackUri</span><span class="sxs-lookup"><span data-stu-id="94fda-142">callbackUri</span></span>       |<span data-ttu-id="94fda-143">String</span><span class="sxs-lookup"><span data-stu-id="94fda-143">String</span></span>                                    |<span data-ttu-id="94fda-144">Permite que os bots forneçam um URI de retorno de chamada específico para que a chamada atual receba notificações posteriores.</span><span class="sxs-lookup"><span data-stu-id="94fda-144">Allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="94fda-145">Se essa propriedade não tiver sido definida, o URI de retorno de chamada global do bot será usado em seu lugar.</span><span class="sxs-lookup"><span data-stu-id="94fda-145">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="94fda-146">Deve ser `https` .</span><span class="sxs-lookup"><span data-stu-id="94fda-146">This must be `https`.</span></span>    |
|<span data-ttu-id="94fda-147">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="94fda-147">acceptedModalities</span></span>|<span data-ttu-id="94fda-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="94fda-148">String collection</span></span>                         |<span data-ttu-id="94fda-149">A lista de aceitar modalidades.</span><span class="sxs-lookup"><span data-stu-id="94fda-149">The list of accept modalities.</span></span> <span data-ttu-id="94fda-150">O valor possível são: `audio` , `video` , `videoBasedScreenSharing` .</span><span class="sxs-lookup"><span data-stu-id="94fda-150">Possible value are: `audio`, `video`, `videoBasedScreenSharing`.</span></span> <span data-ttu-id="94fda-151">Obrigatório para responder a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="94fda-151">Required for answering a call.</span></span> |
|<span data-ttu-id="94fda-152">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="94fda-152">mediaConfig</span></span>       | <span data-ttu-id="94fda-153">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) ou [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="94fda-153">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) or [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span></span> |<span data-ttu-id="94fda-154">A configuração de mídia.</span><span class="sxs-lookup"><span data-stu-id="94fda-154">The media configuration.</span></span> <span data-ttu-id="94fda-155">Precisam</span><span class="sxs-lookup"><span data-stu-id="94fda-155">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="94fda-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="94fda-156">Response</span></span>
<span data-ttu-id="94fda-157">Este método retorna um `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="94fda-157">This method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="94fda-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="94fda-158">Examples</span></span>
<span data-ttu-id="94fda-159">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="94fda-159">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="94fda-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94fda-160">Request</span></span>
<span data-ttu-id="94fda-161">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="94fda-161">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94fda-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="94fda-162">HTTP</span></span>](#tab/http)
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
<span data-ttu-id="94fda-163">Este blob é a configuração serializada para sessões de mídia que é gerada a partir do SDK de mídia.</span><span class="sxs-lookup"><span data-stu-id="94fda-163">This blob is the serialized configuration for media sessions which is generated from the media SDK.</span></span>

# <a name="c"></a>[<span data-ttu-id="94fda-164">C#</span><span class="sxs-lookup"><span data-stu-id="94fda-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94fda-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94fda-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94fda-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94fda-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="94fda-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="94fda-167">Response</span></span>
<span data-ttu-id="94fda-168">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94fda-168">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="94fda-169">Exemplo 1: responder a uma chamada VoIP ponto a ponto com mídia hospedada no serviço</span><span class="sxs-lookup"><span data-stu-id="94fda-169">Example 1: Answer a Peer-to-Peer VoIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="94fda-170">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="94fda-170">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="94fda-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94fda-171">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="94fda-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="94fda-172">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="94fda-173">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="94fda-173">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="94fda-174">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="94fda-174">Notification - established</span></span>

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

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="94fda-175">Exemplo 2: responder a chamada VOIP com mídia hospedada por aplicativo</span><span class="sxs-lookup"><span data-stu-id="94fda-175">Example 2: Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="94fda-176">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="94fda-176">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="94fda-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94fda-177">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="94fda-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="94fda-178">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="94fda-179">C#</span><span class="sxs-lookup"><span data-stu-id="94fda-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94fda-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94fda-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94fda-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94fda-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="94fda-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="94fda-182">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="94fda-183">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="94fda-183">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="94fda-184">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="94fda-184">Notification - established</span></span>

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

### <a name="example-3-answer-a-policy-based-recording-call"></a><span data-ttu-id="94fda-185">Exemplo 3: responder a uma chamada de gravação baseada em política</span><span class="sxs-lookup"><span data-stu-id="94fda-185">Example 3: Answer a policy-based recording call</span></span>

<span data-ttu-id="94fda-186">Sob o [cenário de gravação baseado em políticas](/microsoftteams/teams-recording-policy), antes que um participante da política ingresse em uma chamada, uma notificação de chamada de entrada será enviada ao bot associado à política.</span><span class="sxs-lookup"><span data-stu-id="94fda-186">Under the [Policy-based recording scenario](/microsoftteams/teams-recording-policy), before a participant under policy joins a call, an incoming call notification will be sent to the bot associated with the policy.</span></span>
<span data-ttu-id="94fda-187">As informações de junção podem ser encontradas na propriedade **botData** .</span><span class="sxs-lookup"><span data-stu-id="94fda-187">The join information can be found under the **botData** property.</span></span> <span data-ttu-id="94fda-188">O bot pode optar por responder à chamada e [atualizar o status da gravação de](call-updaterecordingstatus.md) acordo.</span><span class="sxs-lookup"><span data-stu-id="94fda-188">The bot can then choose to answer the call and [update the recording status](call-updaterecordingstatus.md) accordingly.</span></span>

<span data-ttu-id="94fda-189">Veja a seguir um exemplo da notificação de chamada de entrada que um bot receberia nesse caso.</span><span class="sxs-lookup"><span data-stu-id="94fda-189">The following is an example of the incoming call notification that a bot would recieve in this case.</span></span>

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