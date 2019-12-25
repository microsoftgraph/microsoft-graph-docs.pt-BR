---
title: 'Call: resposta'
description: Atenda às chamadas recebidas.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ab0380bca750f53e4f89c32c072843fd53849675
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868286"
---
# <a name="call-answer"></a><span data-ttu-id="e90b0-103">Call: resposta</span><span class="sxs-lookup"><span data-stu-id="e90b0-103">call: answer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e90b0-104">Habilite um bot para atender a uma [chamada](../resources/call.md)de entrada.</span><span class="sxs-lookup"><span data-stu-id="e90b0-104">Enable a bot to answer an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="e90b0-105">A solicitação de chamada de entrada pode ser um convite de um participante em uma chamada de grupo ou uma chamada ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="e90b0-105">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="e90b0-106">Se for recebido um convite para uma chamada de grupo, a notificação conterá os parâmetros [chatInfo](../resources/chatinfo.md) e [meetingInfo](../resources/meetinginfo.md) .</span><span class="sxs-lookup"><span data-stu-id="e90b0-106">If an invite to a group call is received, the notification will contain the [chatInfo](../resources/chatinfo.md) and [meetingInfo](../resources/meetinginfo.md) parameters.</span></span>

<span data-ttu-id="e90b0-107">O bot deve responder, [rejeitar](./call-reject.md) ou [redirecionar](./call-redirect.md) a chamada antes que a chamada expire. O valor de tempo limite atual é de 15 segundos.</span><span class="sxs-lookup"><span data-stu-id="e90b0-107">The bot is expected to answer, [reject](./call-reject.md) or [redirect](./call-redirect.md) the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="e90b0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e90b0-108">Permissions</span></span>
<span data-ttu-id="e90b0-109">Você não precisa de nenhuma permissão para responder a uma chamada ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="e90b0-109">You do not need any permissions to answer a peer-to-peer call.</span></span> <span data-ttu-id="e90b0-110">Você precisa de uma das seguintes permissões para ingressar em uma chamada de grupo.</span><span class="sxs-lookup"><span data-stu-id="e90b0-110">You need one of the following permissions to join a group call.</span></span> <span data-ttu-id="e90b0-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e90b0-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e90b0-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e90b0-112">Permission type</span></span> | <span data-ttu-id="e90b0-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e90b0-113">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="e90b0-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e90b0-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e90b0-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="e90b0-115">Not Supported</span></span>                        |
| <span data-ttu-id="e90b0-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e90b0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e90b0-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="e90b0-117">Not Supported</span></span>                        |
| <span data-ttu-id="e90b0-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e90b0-118">Application</span></span>     | <span data-ttu-id="e90b0-119">Calls. JoinGroupCalls. All ou calls. JoinGroupCallsasGuest. All</span><span class="sxs-lookup"><span data-stu-id="e90b0-119">Calls.JoinGroupCalls.All or Calls.JoinGroupCallsasGuest.All</span></span> |

> <span data-ttu-id="e90b0-120">**Observação:** Para uma chamada que usa mídia hospedada por aplicativo, você também precisa da permissão calls. AccessMedia. All.</span><span class="sxs-lookup"><span data-stu-id="e90b0-120">**Note:** For a call that uses application-hosted media, you also need the Calls.AccessMedia.All permission.</span></span> <span data-ttu-id="e90b0-121">Você deve ter pelo menos uma das seguintes permissões para garantir que o `source` na notificação de chamada de entrada seja descriptografado: calls. AccessMedia. All, calls. initiate. All, calls. InitiateGroupCall. All, calls. JoinGroupCall. All, calls. JoinGroupCallAsGuest. All.</span><span class="sxs-lookup"><span data-stu-id="e90b0-121">You must have at least one of the following permissions to ensure that the `source` in the incoming call notification is decrypted: Calls.AccessMedia.All, Calls.Initiate.All, Calls.InitiateGroupCall.All, Calls.JoinGroupCall.All, Calls.JoinGroupCallAsGuest.All.</span></span> <span data-ttu-id="e90b0-122">O `source` é a informação do chamador na notificação de chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="e90b0-122">The `source` is the caller info in the incoming call notification.</span></span> <span data-ttu-id="e90b0-123">Sem pelo menos uma dessas permissões, o `source` permanecerá criptografado.</span><span class="sxs-lookup"><span data-stu-id="e90b0-123">Without at least one of these permissions, the `source` will remain encrypted.</span></span>

## <a name="http-request"></a><span data-ttu-id="e90b0-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e90b0-124">HTTP request</span></span>
<!-- {"blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /communications/calls/{id}/answer
```
> <span data-ttu-id="e90b0-125">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="e90b0-125">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="e90b0-126">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="e90b0-126">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e90b0-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e90b0-127">Request headers</span></span>
| <span data-ttu-id="e90b0-128">Nome</span><span class="sxs-lookup"><span data-stu-id="e90b0-128">Name</span></span>          | <span data-ttu-id="e90b0-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="e90b0-129">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e90b0-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="e90b0-130">Authorization</span></span> | <span data-ttu-id="e90b0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e90b0-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e90b0-133">Content-type</span><span class="sxs-lookup"><span data-stu-id="e90b0-133">Content-type</span></span>  | <span data-ttu-id="e90b0-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e90b0-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e90b0-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e90b0-136">Request body</span></span>
<span data-ttu-id="e90b0-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e90b0-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e90b0-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e90b0-138">Parameter</span></span>        | <span data-ttu-id="e90b0-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="e90b0-139">Type</span></span>                                     |<span data-ttu-id="e90b0-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="e90b0-140">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="e90b0-141">callbackUri</span><span class="sxs-lookup"><span data-stu-id="e90b0-141">callbackUri</span></span>       |<span data-ttu-id="e90b0-142">String</span><span class="sxs-lookup"><span data-stu-id="e90b0-142">String</span></span>                                    |<span data-ttu-id="e90b0-143">Permite que os bots forneçam um URI de retorno de chamada específico para que a chamada atual receba notificações posteriores.</span><span class="sxs-lookup"><span data-stu-id="e90b0-143">Allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="e90b0-144">Se essa propriedade não tiver sido definida, o URI de retorno de chamada global do bot será usado em seu lugar.</span><span class="sxs-lookup"><span data-stu-id="e90b0-144">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="e90b0-145">Deve ser `https`.</span><span class="sxs-lookup"><span data-stu-id="e90b0-145">This must be `https`.</span></span>    |
|<span data-ttu-id="e90b0-146">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="e90b0-146">acceptedModalities</span></span>|<span data-ttu-id="e90b0-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e90b0-147">String collection</span></span>                         |<span data-ttu-id="e90b0-148">A lista de aceitar modalidades.</span><span class="sxs-lookup"><span data-stu-id="e90b0-148">The list of accept modalities.</span></span> <span data-ttu-id="e90b0-149">O valor possível são `audio`: `video`, `videoBasedScreenSharing`,.</span><span class="sxs-lookup"><span data-stu-id="e90b0-149">Possible value are: `audio`, `video`, `videoBasedScreenSharing`.</span></span> <span data-ttu-id="e90b0-150">Obrigatório para responder a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="e90b0-150">Required for answering a call.</span></span> |
|<span data-ttu-id="e90b0-151">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="e90b0-151">mediaConfig</span></span>       | <span data-ttu-id="e90b0-152">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) ou [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="e90b0-152">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) or [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span></span> |<span data-ttu-id="e90b0-153">A configuração de mídia.</span><span class="sxs-lookup"><span data-stu-id="e90b0-153">The media configuration.</span></span> <span data-ttu-id="e90b0-154">Precisam</span><span class="sxs-lookup"><span data-stu-id="e90b0-154">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="e90b0-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="e90b0-155">Response</span></span>
<span data-ttu-id="e90b0-156">Este método retorna um `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="e90b0-156">This method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e90b0-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e90b0-157">Examples</span></span>
<span data-ttu-id="e90b0-158">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e90b0-158">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e90b0-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e90b0-159">Request</span></span>
<span data-ttu-id="e90b0-160">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="e90b0-160">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e90b0-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="e90b0-161">HTTP</span></span>](#tab/http)
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
<span data-ttu-id="e90b0-162">Este blob é a configuração serializada para sessões de mídia que é gerada a partir do SDK de mídia.</span><span class="sxs-lookup"><span data-stu-id="e90b0-162">This blob is the serialized configuration for media sessions which is generated from the media SDK.</span></span>

# <a name="ctabcsharp"></a>[<span data-ttu-id="e90b0-163">C#</span><span class="sxs-lookup"><span data-stu-id="e90b0-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e90b0-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e90b0-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e90b0-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e90b0-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e90b0-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="e90b0-166">Response</span></span>
<span data-ttu-id="e90b0-167">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e90b0-167">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="e90b0-168">Exemplo 1: responder a uma chamada VoIP ponto a ponto com mídia hospedada no serviço</span><span class="sxs-lookup"><span data-stu-id="e90b0-168">Example 1: Answer a Peer-to-Peer VoIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="e90b0-169">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="e90b0-169">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="e90b0-170">Solicitar</span><span class="sxs-lookup"><span data-stu-id="e90b0-170">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="e90b0-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="e90b0-171">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="e90b0-172">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="e90b0-172">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="e90b0-173">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="e90b0-173">Notification - established</span></span>

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

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="e90b0-174">Exemplo 2: responder a chamada VOIP com mídia hospedada por aplicativo</span><span class="sxs-lookup"><span data-stu-id="e90b0-174">Example 2: Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="e90b0-175">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="e90b0-175">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="e90b0-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e90b0-176">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e90b0-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="e90b0-177">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e90b0-178">C#</span><span class="sxs-lookup"><span data-stu-id="e90b0-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e90b0-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e90b0-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e90b0-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e90b0-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e90b0-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="e90b0-181">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="e90b0-182">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="e90b0-182">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="e90b0-183">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="e90b0-183">Notification - established</span></span>

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
