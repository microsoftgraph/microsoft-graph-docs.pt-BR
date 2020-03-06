---
title: 'Call: resposta'
description: Atenda às chamadas recebidas.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ca7cfb0a8f1851727138a21e92a3df8a2b968513
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518743"
---
# <a name="call-answer"></a><span data-ttu-id="848f3-103">Call: resposta</span><span class="sxs-lookup"><span data-stu-id="848f3-103">call: answer</span></span>

<span data-ttu-id="848f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="848f3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="848f3-105">Habilite um bot para atender a uma [chamada](../resources/call.md)de entrada.</span><span class="sxs-lookup"><span data-stu-id="848f3-105">Enable a bot to answer an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="848f3-106">A solicitação de chamada de entrada pode ser um convite de um participante em uma chamada de grupo ou uma chamada ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="848f3-106">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="848f3-107">Se for recebido um convite para uma chamada de grupo, a notificação conterá os parâmetros [chatInfo](../resources/chatinfo.md) e [meetingInfo](../resources/meetinginfo.md) .</span><span class="sxs-lookup"><span data-stu-id="848f3-107">If an invite to a group call is received, the notification will contain the [chatInfo](../resources/chatinfo.md) and [meetingInfo](../resources/meetinginfo.md) parameters.</span></span>

<span data-ttu-id="848f3-108">O bot deve responder, [rejeitar](./call-reject.md)ou [redirecionar](./call-redirect.md) a chamada antes do tempo limite da chamada. O valor de tempo limite atual é de 15 segundos.</span><span class="sxs-lookup"><span data-stu-id="848f3-108">The bot is expected to answer, [reject](./call-reject.md), or [redirect](./call-redirect.md) the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="848f3-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="848f3-109">Permissions</span></span>
<span data-ttu-id="848f3-110">Você não precisa de nenhuma permissão para responder a uma chamada ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="848f3-110">You do not need any permissions to answer a peer-to-peer call.</span></span> <span data-ttu-id="848f3-111">Você precisa de uma das seguintes permissões para ingressar em uma chamada de grupo.</span><span class="sxs-lookup"><span data-stu-id="848f3-111">You need one of the following permissions to join a group call.</span></span> <span data-ttu-id="848f3-112">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="848f3-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="848f3-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="848f3-113">Permission type</span></span> | <span data-ttu-id="848f3-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="848f3-114">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="848f3-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="848f3-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="848f3-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="848f3-116">Not Supported</span></span>                        |
| <span data-ttu-id="848f3-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="848f3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="848f3-118">Não suportado</span><span class="sxs-lookup"><span data-stu-id="848f3-118">Not Supported</span></span>                        |
| <span data-ttu-id="848f3-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="848f3-119">Application</span></span>     | <span data-ttu-id="848f3-120">Calls. JoinGroupCalls. All ou calls. JoinGroupCallsasGuest. All</span><span class="sxs-lookup"><span data-stu-id="848f3-120">Calls.JoinGroupCalls.All or Calls.JoinGroupCallsasGuest.All</span></span> |

> <span data-ttu-id="848f3-121">**Observação:** Para uma chamada que usa mídia hospedada por aplicativo, você também precisa da permissão calls. AccessMedia. All.</span><span class="sxs-lookup"><span data-stu-id="848f3-121">**Note:** For a call that uses application-hosted media, you also need the Calls.AccessMedia.All permission.</span></span> <span data-ttu-id="848f3-122">Você deve ter pelo menos uma das seguintes permissões para garantir que o `source` na notificação de chamada de entrada seja descriptografado: calls. AccessMedia. All, calls. initiate. All, calls. InitiateGroupCall. All, calls. JoinGroupCall. All, calls. JoinGroupCallAsGuest. All.</span><span class="sxs-lookup"><span data-stu-id="848f3-122">You must have at least one of the following permissions to ensure that the `source` in the incoming call notification is decrypted: Calls.AccessMedia.All, Calls.Initiate.All, Calls.InitiateGroupCall.All, Calls.JoinGroupCall.All, Calls.JoinGroupCallAsGuest.All.</span></span> <span data-ttu-id="848f3-123">O `source` é a informação do chamador na notificação de chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="848f3-123">The `source` is the caller info in the incoming call notification.</span></span> <span data-ttu-id="848f3-124">Sem pelo menos uma dessas permissões, o `source` permanecerá criptografado.</span><span class="sxs-lookup"><span data-stu-id="848f3-124">Without at least one of these permissions, the `source` will remain encrypted.</span></span>

## <a name="http-request"></a><span data-ttu-id="848f3-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="848f3-125">HTTP request</span></span>
<!-- {"blockType": "ignored" } -->
```http
POST /communications/calls/{id}/answer
```

## <a name="request-headers"></a><span data-ttu-id="848f3-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="848f3-126">Request headers</span></span>
| <span data-ttu-id="848f3-127">Nome</span><span class="sxs-lookup"><span data-stu-id="848f3-127">Name</span></span>          | <span data-ttu-id="848f3-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="848f3-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="848f3-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="848f3-129">Authorization</span></span> | <span data-ttu-id="848f3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="848f3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="848f3-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="848f3-132">Content-type</span></span>  | <span data-ttu-id="848f3-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="848f3-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="848f3-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="848f3-135">Request body</span></span>
<span data-ttu-id="848f3-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="848f3-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="848f3-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="848f3-137">Parameter</span></span>        | <span data-ttu-id="848f3-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="848f3-138">Type</span></span>                                     |<span data-ttu-id="848f3-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="848f3-139">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="848f3-140">callbackUri</span><span class="sxs-lookup"><span data-stu-id="848f3-140">callbackUri</span></span>       |<span data-ttu-id="848f3-141">String</span><span class="sxs-lookup"><span data-stu-id="848f3-141">String</span></span>                                    |<span data-ttu-id="848f3-142">Permite que os bots forneçam um URI de retorno de chamada específico para que a chamada atual receba notificações posteriores.</span><span class="sxs-lookup"><span data-stu-id="848f3-142">Allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="848f3-143">Se essa propriedade não tiver sido definida, o URI de retorno de chamada global do bot será usado em seu lugar.</span><span class="sxs-lookup"><span data-stu-id="848f3-143">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="848f3-144">Deve ser `https`.</span><span class="sxs-lookup"><span data-stu-id="848f3-144">This must be `https`.</span></span>    |
|<span data-ttu-id="848f3-145">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="848f3-145">acceptedModalities</span></span>|<span data-ttu-id="848f3-146">String collection</span><span class="sxs-lookup"><span data-stu-id="848f3-146">String collection</span></span>                         |<span data-ttu-id="848f3-147">A lista de aceitar modalidades.</span><span class="sxs-lookup"><span data-stu-id="848f3-147">The list of accept modalities.</span></span> <span data-ttu-id="848f3-148">Os valores possíveis são: `audio`, `video`, `videoBasedScreenSharing`.</span><span class="sxs-lookup"><span data-stu-id="848f3-148">Possible values are: `audio`, `video`, `videoBasedScreenSharing`.</span></span> <span data-ttu-id="848f3-149">Obrigatório para responder a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="848f3-149">Required for answering a call.</span></span> |
|<span data-ttu-id="848f3-150">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="848f3-150">mediaConfig</span></span>       | <span data-ttu-id="848f3-151">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) ou [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="848f3-151">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) or [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span></span> |<span data-ttu-id="848f3-152">A configuração de mídia.</span><span class="sxs-lookup"><span data-stu-id="848f3-152">The media configuration.</span></span> <span data-ttu-id="848f3-153">Precisam</span><span class="sxs-lookup"><span data-stu-id="848f3-153">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="848f3-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="848f3-154">Response</span></span>
<span data-ttu-id="848f3-155">Este método retorna um `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="848f3-155">This method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="848f3-156">Exemplos</span><span class="sxs-lookup"><span data-stu-id="848f3-156">Examples</span></span>
<span data-ttu-id="848f3-157">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="848f3-157">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="848f3-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="848f3-158">Request</span></span>
<span data-ttu-id="848f3-159">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="848f3-159">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="848f3-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="848f3-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-answer"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/answer
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
<span data-ttu-id="848f3-161">Este blob é a configuração serializada para sessões de mídia que é gerada a partir do SDK de mídia.</span><span class="sxs-lookup"><span data-stu-id="848f3-161">This blob is the serialized configuration for media sessions which is generated from the media SDK.</span></span>

# <a name="c"></a>[<span data-ttu-id="848f3-162">C#</span><span class="sxs-lookup"><span data-stu-id="848f3-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="848f3-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="848f3-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="848f3-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="848f3-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="848f3-165">Java</span><span class="sxs-lookup"><span data-stu-id="848f3-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="848f3-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="848f3-166">Response</span></span>
<span data-ttu-id="848f3-167">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="848f3-167">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="848f3-168">Exemplo 1: responder a uma chamada VoIP ponto a ponto com mídia hospedada no serviço</span><span class="sxs-lookup"><span data-stu-id="848f3-168">Example 1: Answer a Peer-to-Peer VoIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="848f3-169">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="848f3-169">Notification - incoming</span></span>

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
            }
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="848f3-170">Solicitar</span><span class="sxs-lookup"><span data-stu-id="848f3-170">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="848f3-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="848f3-171">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="848f3-172">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="848f3-172">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="848f3-173">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="848f3-173">Notification - established</span></span>

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

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="848f3-174">Exemplo 2: responder a chamada VOIP com mídia hospedada por aplicativo</span><span class="sxs-lookup"><span data-stu-id="848f3-174">Example 2: Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="848f3-175">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="848f3-175">Notification - incoming</span></span>

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
            }
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="848f3-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="848f3-176">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="848f3-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="848f3-177">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="848f3-178">C#</span><span class="sxs-lookup"><span data-stu-id="848f3-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="848f3-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="848f3-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="848f3-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="848f3-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="848f3-181">Java</span><span class="sxs-lookup"><span data-stu-id="848f3-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="848f3-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="848f3-182">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="848f3-183">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="848f3-183">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="848f3-184">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="848f3-184">Notification - established</span></span>

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
