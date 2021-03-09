---
title: Criar chamada
description: Crie uma nova chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 888fb523ad54f840b5ecbc807b5ed46c8f798efb
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574899"
---
# <a name="create-call"></a><span data-ttu-id="eb237-103">Criar chamada</span><span class="sxs-lookup"><span data-stu-id="eb237-103">Create call</span></span>

<span data-ttu-id="eb237-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb237-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb237-105">Criar [chamada](../resources/call.md) permite que seu bot crie uma nova chamada ponto a ponto ou grupo de saída ou participe de uma reunião existente.</span><span class="sxs-lookup"><span data-stu-id="eb237-105">Create [call](../resources/call.md) enables your bot to create a new outgoing peer-to-peer or group call, or join an existing meeting.</span></span> <span data-ttu-id="eb237-106">Você precisará registrar [o bot de chamada](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) e passar pela lista de permissões necessárias, conforme mencionado abaixo.</span><span class="sxs-lookup"><span data-stu-id="eb237-106">You will need to [register the calling bot](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) and go through the list of permissions needed as mentioned below.</span></span>

> <span data-ttu-id="eb237-107">**Observação:** Atualmente, apenas chamadas VoIP são suportadas.</span><span class="sxs-lookup"><span data-stu-id="eb237-107">**Note:** Currently, only VoIP calls are supported.</span></span> 

## <a name="permissions"></a><span data-ttu-id="eb237-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb237-108">Permissions</span></span>

<span data-ttu-id="eb237-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span><span class="sxs-lookup"><span data-stu-id="eb237-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span></span>

| <span data-ttu-id="eb237-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb237-111">Permission type</span></span>                        | <span data-ttu-id="eb237-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb237-112">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="eb237-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb237-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb237-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="eb237-114">Not Supported</span></span>                                                                           |
| <span data-ttu-id="eb237-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb237-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb237-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="eb237-116">Not Supported</span></span>                                                                           |
| <span data-ttu-id="eb237-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb237-117">Application</span></span>                            | <span data-ttu-id="eb237-118">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate. All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="eb237-118">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="eb237-119">**Observação:** Para uma chamada com a mídia hospedada pelo aplicativo, você precisa da permissão Calls.AccessMedia.All, além de uma das permissões listadas.</span><span class="sxs-lookup"><span data-stu-id="eb237-119">**Note:** For a call with app-hosted media, you need the Calls.AccessMedia.All permission in addition to one of the permissions listed.</span></span>

## <a name="http-request"></a><span data-ttu-id="eb237-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb237-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
POST /communications/calls
```
> <span data-ttu-id="eb237-121">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="eb237-121">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="eb237-122">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="eb237-122">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb237-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb237-123">Request headers</span></span>
| <span data-ttu-id="eb237-124">Nome</span><span class="sxs-lookup"><span data-stu-id="eb237-124">Name</span></span>          | <span data-ttu-id="eb237-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb237-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="eb237-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb237-126">Authorization</span></span> | <span data-ttu-id="eb237-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb237-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eb237-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="eb237-129">Content-type</span></span>  | <span data-ttu-id="eb237-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb237-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb237-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb237-132">Request body</span></span>
<span data-ttu-id="eb237-133">No corpo da solicitação, fornece uma representação JSON de um [objeto de](../resources/call.md) chamada.</span><span class="sxs-lookup"><span data-stu-id="eb237-133">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="eb237-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb237-134">Response</span></span>
<span data-ttu-id="eb237-135">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto de](../resources/call.md) chamada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb237-135">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb237-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eb237-136">Examples</span></span>

### <a name="example-1-create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="eb237-137">Exemplo 1: Criar chamada VoIP ponto a ponto com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="eb237-137">Example 1: Create peer-to-peer VoIP call with service hosted media</span></span>

> <span data-ttu-id="eb237-138">**Observação:** Essa chamada precisa da Calls.Initiate. Todas as permissões.</span><span class="sxs-lookup"><span data-stu-id="eb237-138">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="eb237-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb237-139">Request</span></span>
<span data-ttu-id="eb237-140">O exemplo a seguir mostra a solicitação que faz uma chamada ponto a ponto entre o bot e o usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="eb237-140">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="eb237-141">Neste exemplo, a mídia é hospedada pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="eb237-141">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="eb237-142">Os valores de token de autorização, URL de retorno de chamada, ID do aplicativo, nome do aplicativo, ID de usuário, nome de usuário e ID de locatário devem ser substituídos por valores reais para fazer o exemplo funcionar.</span><span class="sxs-lookup"><span data-stu-id="eb237-142">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="eb237-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb237-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "John",
          "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig"
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="eb237-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb237-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-service-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="eb237-145">C#</span><span class="sxs-lookup"><span data-stu-id="eb237-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-service-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb237-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb237-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-service-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb237-147">Java</span><span class="sxs-lookup"><span data-stu-id="eb237-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-service-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eb237-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb237-148">Response</span></span>

> <span data-ttu-id="eb237-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="eb237-149">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
      }
    },
    "countryCode": null,
    "endpointType": null,
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "John",
          "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      },
      "endpointType": null,
      "region": null,
      "replacesCallId": null,
      "languageId": null
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "activeModalities": [],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "routingPolicies": [],
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#app/calls/$entity",
  "subject": null,
  "terminationReason": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="eb237-150">Notificação - estabelecimento</span><span class="sxs-lookup"><span data-stu-id="eb237-150">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/callback
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
      "resourceUrl": "/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "establishing",
        "id": "2e1a0b00-2db4-4022-9570-243709c565ab"
      }
    }
  ]
}
```
##### <a name="notification---established"></a><span data-ttu-id="eb237-151">Notificação - estabelecida</span><span class="sxs-lookup"><span data-stu-id="eb237-151">Notification - established</span></span>

```http
POST https://bot.contoso.com/callback
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
      "resourceUrl": "/communications/calls/2e1a0b00-b3c5-4b0f-99b3-c133bc1e6116",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "direction": "outgoing",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "id": "2e1a0b00-b3c5-4b0f-99b3-c133bc1e6116"
      }
    }
  ]
}
```

### <a name="example-2-create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="eb237-152">Exemplo 2: Criar chamada VoIP ponto a ponto com mídia hospedada por aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb237-152">Example 2: Create peer-to-peer VoIP call with application hosted media</span></span>

> <span data-ttu-id="eb237-153">**Observação**: este exemplo precisa Calls.Initiate. Permissões All e Calls.AccessMedia.All.</span><span class="sxs-lookup"><span data-stu-id="eb237-153">**Note**: This example needs Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="eb237-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb237-154">Request</span></span>
<span data-ttu-id="eb237-155">O exemplo a seguir mostra a solicitação que faz uma chamada ponto a ponto entre o bot e o usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="eb237-155">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="eb237-156">Neste exemplo, a mídia é hospedada localmente pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eb237-156">In this example the media is hosted locally by the application.</span></span> <span data-ttu-id="eb237-157">Os valores de token de autorização, url de retorno de chamada, id do aplicativo, nome do aplicativo, id de usuário, nome de usuário e id de locatário devem ser substituídos por valores reais para fazer o exemplo funcionar.</span><span class="sxs-lookup"><span data-stu-id="eb237-157">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="eb237-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb237-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-app-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
      }
    },
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "John",
          "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
 "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="eb237-159">C#</span><span class="sxs-lookup"><span data-stu-id="eb237-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb237-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb237-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb237-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb237-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb237-162">Java</span><span class="sxs-lookup"><span data-stu-id="eb237-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="eb237-163">`<Media Session Configuration>` é a configuração de sessão de mídia serializada que contém as informações de sessão da pilha de mídia.</span><span class="sxs-lookup"><span data-stu-id="eb237-163">`<Media Session Configuration>` is the serialized media session configuration which contains the session information of the media stack.</span></span> <span data-ttu-id="eb237-164">Informações específicas sobre áudio, vídeo, informações de ssession VBSS devem ser passadas aqui.</span><span class="sxs-lookup"><span data-stu-id="eb237-164">Specific information about audio, video, VBSS ssession information should be passed here.</span></span>

<span data-ttu-id="eb237-165">Exemplo de blob de sessão de mídia de áudio é mostrado abaixo</span><span class="sxs-lookup"><span data-stu-id="eb237-165">Sample audio media session blob is shown below</span></span>
```json
{\"mpUri\":\"net.tcp://bot.contoso.com:18732/MediaProcessor\",\"audioRenderContexts\":[\"14778cc4-f54c-43c7-989f-9092e34ef784\"],\"videoRenderContexts\":[],\"audioSourceContexts\":[\"a5dcfc9b-5a54-48ef-86f5-1fdd8508741a\"],\"videoSourceContexts\":[],\"dataRenderContexts\":null,\"dataSourceContexts\":null,\"supportedAudioFormat\":\"Pcm16K\",\"videoSinkEncodingFormats\":[],\"mpMediaSessionId\":\"2379cf46-acf3-4fef-a914-be9627075320\",\"regionAffinity\":null,\"skypeMediaBotsVersion\":\"1.11.1.0086\",\"mediaStackVersion\":\"2018.53.1.1\",\"mpVersion\":\"7.2.0.3881\",\"callId\":\"1b69b141-7f1a-4033-9c34-202737190a20\"}
```

><span data-ttu-id="eb237-166">**Observação:** Para chamadas ponto a ponto, as notificações esperadas são apenas para alterações de estado de chamada.</span><span class="sxs-lookup"><span data-stu-id="eb237-166">**Note:** For peer-to-peer calls, the expected notifications are for call state changes only.</span></span>

##### <a name="response"></a><span data-ttu-id="eb237-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb237-167">Response</span></span>

> <span data-ttu-id="eb237-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb237-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
      }
    },
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "John",
          "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "activeModalities": [],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>",
  },
  "routingPolicies": [],
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#app/calls/$entity",
  "subject": null,
  "terminationReason": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

### <a name="example-3-create-a-group-call-with-service-hosted-media"></a><span data-ttu-id="eb237-170">Exemplo 3: Criar uma chamada de grupo com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="eb237-170">Example 3: Create a group call with service hosted media</span></span>

<span data-ttu-id="eb237-171">Isso dá suporte a até 5 usuários VoIP.</span><span class="sxs-lookup"><span data-stu-id="eb237-171">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="eb237-172">O exemplo mostra como criar uma chamada de grupo com dois usuários VoIP.</span><span class="sxs-lookup"><span data-stu-id="eb237-172">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="eb237-173">**Observação:** Esta chamada de exemplo precisa da `Calls.InitiateGroupCalls.All` permissão.</span><span class="sxs-lookup"><span data-stu-id="eb237-173">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="eb237-174">A chamada de grupo criada não dá suporte a chat ou gravação.</span><span class="sxs-lookup"><span data-stu-id="eb237-174">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="eb237-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb237-175">Request</span></span>
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json
```
<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "@odata.type": "#microsoft.graph.call",
  "direction": "outgoing",
  "subject": "Create a group call with service hosted media",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "TestBot",
        "id": "dd3885da-f9ab-486b-bfae-85de3d445555"
      }
    }
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "user1",
          "id": "98da8a1a-1b87-452c-a713-65d3f10b5555"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.participantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "user2",
          "id": "bf5aae9a-d11d-47a8-93b1-782504c95555"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "removeFromDefaultAudioGroup": false
  },
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a"
}
```

### <a name="example-4-create-a-group-call-with-application-hosted-media"></a><span data-ttu-id="eb237-176">Exemplo 4: Criar uma chamada de grupo com mídia hospedada por aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb237-176">Example 4: Create a group call with application hosted media</span></span>

<span data-ttu-id="eb237-177">Isso dá suporte a até 5 usuários VoIP.</span><span class="sxs-lookup"><span data-stu-id="eb237-177">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="eb237-178">O exemplo mostra como criar uma chamada de grupo com dois usuários VoIP.</span><span class="sxs-lookup"><span data-stu-id="eb237-178">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="eb237-179">**Observação:** Esta chamada de exemplo precisa da `Calls.InitiateGroupCalls.All` permissão.</span><span class="sxs-lookup"><span data-stu-id="eb237-179">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="eb237-180">A chamada de grupo criada não dá suporte a chat ou gravação.</span><span class="sxs-lookup"><span data-stu-id="eb237-180">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="eb237-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb237-181">Request</span></span>
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json
```
<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "@odata.type": "#microsoft.graph.call",
  "direction": "outgoing",
  "subject": "Create a group call with service hosted media",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "TestBot",
        "id": "dd3885da-f9ab-486b-bfae-85de3d445555"
      }
    }
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "user1",
          "id": "98da8a1a-1b87-452c-a713-65d3f10b5555"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.participantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "user2",
          "id": "bf5aae9a-d11d-47a8-93b1-782504c95555"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>",
    "removeFromDefaultAudioGroup": false
  },
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a"
}
```

### <a name="example-5-join-scheduled-meeting-with-service-hosted-media"></a><span data-ttu-id="eb237-182">Exemplo 5: Participar de reunião agendada com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="eb237-182">Example 5: Join scheduled meeting with service hosted media</span></span>
<span data-ttu-id="eb237-183">Para participar da reunião agendada, precisamos obter a ID do thread, a ID da mensagem, a ID do organizador e a id do locatário na qual a reunião está agendada.</span><span class="sxs-lookup"><span data-stu-id="eb237-183">To join the scheduled meeting we will need to get the thread id, message id, organizer id and the tenant id in which the meeting is scheduled.</span></span>
<span data-ttu-id="eb237-184">Essas informações podem ser obtidas da [API Obter Reuniões Online.](../api/onlinemeeting-get.md)</span><span class="sxs-lookup"><span data-stu-id="eb237-184">This information can be obtained from [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="eb237-185">Os valores de token de autorização, url de retorno de chamada, id de aplicativo, nome do aplicativo, id de usuário, nome de usuário e id de locatário devem ser substituídos juntamente com os detalhes obtidos da  [API De](../api/onlinemeeting-get.md) Reuniões Get Online com valores reais para fazer o exemplo funcionar.</span><span class="sxs-lookup"><span data-stu-id="eb237-185">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>
> <span data-ttu-id="eb237-186">**Observação:** Este exemplo precisa da `Calls.JoinGroupCalls.All` permissão.</span><span class="sxs-lookup"><span data-stu-id="eb237-186">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="eb237-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb237-187">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="eb237-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb237-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "join-meeting-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
    "messageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "displayName": "Bob",
        "tenantId":"86dc81db-c112-4228-9222-63f3esaa1edb"
      }
    },
    "allowConversationWithoutHost": true
  },
  "tenantId":"86dc81db-c112-4228-9222-63f3esaa1edb"
}
```
# <a name="c"></a>[<span data-ttu-id="eb237-189">C#</span><span class="sxs-lookup"><span data-stu-id="eb237-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/join-meeting-service-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb237-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb237-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/join-meeting-service-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb237-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb237-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/join-meeting-service-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="eb237-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb237-192">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": "true",
  "@odata.type": "microsoft.graph.call"
}-->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
      }
    },
    "region": null,
    "languageId": null
  },
  "targets": [],
  "requestedModalities": [
    "audio"
  ],
  "activeModalities": [],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
    "messageId": "0",
    "replyChainMessageId": null
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  },
  "transcription": null,
  "routingPolicies": [],
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
  "myParticipantId": "05491616-385f-44a8-9974-18cc5f9933c1",
  "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#app/calls/$entity",
  "terminationReason": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "subject": null,
  "resultInfo": null,
  "answeredBy": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="eb237-193">Notificação - estabelecimento</span><span class="sxs-lookup"><span data-stu-id="eb237-193">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/callback
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
      "resourceUrl": "/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92",
        "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "establishing",
        "chatInfo": {
          "@odata.type": "#microsoft.graph.chatInfo",
          "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
          "messageId": "0"
        },
        "meetingInfo": {
          "@odata.type": "#microsoft.graph.organizerMeetingInfo",
          "organizer": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
              "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
              "displayName": "Bob"
            }
          },
          "allowConversationWithoutHost": true
        },
        "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92"
      }
    }
  ]
}

```
##### <a name="notification---established"></a><span data-ttu-id="eb237-194">Notificação - estabelecida</span><span class="sxs-lookup"><span data-stu-id="eb237-194">Notification - established</span></span>

```http
POST https://bot.contoso.com/callback
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
      "resourceUrl": "/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "chatInfo": {
          "@odata.type": "#microsoft.graph.chatInfo",
          "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
          "messageId": "0"
        },
        "meetingInfo": {
          "@odata.type": "#microsoft.graph.organizerMeetingInfo",
          "organizer": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
              "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
              "displayName": "Bob"
            }
          },
          "allowConversationWithoutHost": true
        },
        "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92"
      }
    }
  ]
}
```
##### <a name="notification---roster"></a><span data-ttu-id="eb237-195">Notificação - lista</span><span class="sxs-lookup"><span data-stu-id="eb237-195">Notification - roster</span></span>

```http
POST https://bot.contoso.com/callback
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92/participants",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "John",
                "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
              }
            },
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "sourceId": "1",
              "direction": "sendReceive",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "video",
              "sourceId": "2",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "videoBasedScreenSharing",
              "sourceId": "8",
              "direction": "receiveOnly",
              "serverMuted": false
            }
          ],
          "isMuted": true,
          "isInLobby": false,
          "id": "0d7664b6-6432-43ed-8d27-d9e7adec188c"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "Calling Bot",
                "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
              }
            }
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "sourceId": "10",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "id": "05491616-385f-44a8-9974-18cc5f9933c1"
        }
      ]
    }
  ]
}
```

><span data-ttu-id="eb237-196">**Observação:** Para participar de cenários de reunião, além das notificações de estado de chamada, recebemos notificações de lista.</span><span class="sxs-lookup"><span data-stu-id="eb237-196">**Note:** For join meeting scenarios apart from call state notifications, we receive roster notifications.</span></span>

### <a name="example-6-join-scheduled-meeting-with-app-hosted-media"></a><span data-ttu-id="eb237-197">Exemplo 6: Participar de uma reunião agendada com a mídia hospedada pelo aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb237-197">Example 6: Join scheduled meeting with app hosted media</span></span>
<span data-ttu-id="eb237-198">Para ingressar na reunião com a mídia hospedada no aplicativo, atualize a configuração de mídia com [o AppHostedMediaConfig,](../resources/apphostedmediaconfig.md) conforme mostrado abaixo, no exemplo fornecido acima.</span><span class="sxs-lookup"><span data-stu-id="eb237-198">To join the meeting with application hosted media update the media config with the [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) as shown below, In the sample provided above.</span></span>

<!-- {
  "blockType": "example",
  "name": "join-meeting-app-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>",
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
    "messageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  },
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a"
}
```


### <a name="example-7-join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="eb237-199">Exemplo 7: Participar de reunião de canal com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="eb237-199">Example 7: Join channel meeting with service hosted media</span></span>
<span data-ttu-id="eb237-200">A reunião dentro de um canal requer detalhes específicos, como id de thread, messageid e detalhes do organizador que podem ser obtidos usando a [API Obter Reuniões Online](../api/onlinemeeting-get.md).</span><span class="sxs-lookup"><span data-stu-id="eb237-200">Meeting inside a channel requires specific details like thread id, messageid, and organizer details that can be obtained using the [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="eb237-201">Os valores de token de autorização, url de retorno de chamada, id de aplicativo, nome do aplicativo, id de usuário, nome de usuário e id de locatário devem ser substituídos juntamente com os detalhes obtidos da  [API De](../api/onlinemeeting-get.md) Reuniões Get Online com valores reais para fazer o exemplo funcionar.</span><span class="sxs-lookup"><span data-stu-id="eb237-201">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>

> <span data-ttu-id="eb237-202">**Observação:** Este exemplo precisa da `Calls.JoinGroupCalls.All` permissão.</span><span class="sxs-lookup"><span data-stu-id="eb237-202">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="eb237-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb237-203">Request</span></span>

<!-- {
  "blockType": "example",
  "name": "join-channel-meeting-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
    "messageId": "1533758867081"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  }
}
```

### <a name="example-8-join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="eb237-204">Exemplo 8: participar da reunião do canal como convidado com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="eb237-204">Example 8: Join channel meeting as a guest with service hosted media</span></span>
<span data-ttu-id="eb237-205">Para ingressar em uma reunião de canal como [](../resources/identityset.md) convidado, você precisará criar uma identidade de convidado e adicioná-la como fonte de chamada na solicitação de reunião de participação.</span><span class="sxs-lookup"><span data-stu-id="eb237-205">For joining a channel meeting as a guest you will need to create a guest [identity](../resources/identityset.md) and add it as the call source in the join meeting request.</span></span>
<span data-ttu-id="eb237-206">O nome para exibição é o nome que você deseja exibir na reunião para sua identidade de convidado.</span><span class="sxs-lookup"><span data-stu-id="eb237-206">The display name is the name you want to be displayed in the meeting for your guest identity.</span></span> <span data-ttu-id="eb237-207">A id pode ser uma id exclusiva que identifica a identidade do convidado.</span><span class="sxs-lookup"><span data-stu-id="eb237-207">The id may be a unique id identifying the guest identity.</span></span>

> <span data-ttu-id="eb237-208">**Observação:** Este exemplo precisa da `Calls.JoinGroupCallsAsGuest.All` permissão.</span><span class="sxs-lookup"><span data-stu-id="eb237-208">**Note:** This example needs the `Calls.JoinGroupCallsAsGuest.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="eb237-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb237-209">Request</span></span>

<!-- {
  "blockType": "example",
  "name": "join-channel-meeting-as-guest-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "guest": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Guest User",
        "id": "d7a3b999-17ac-4bca-9e77-e6a730d2ec2e"
      }
    }
  },
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
    "messageId": "1533758867081"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  }
}
```
> <span data-ttu-id="eb237-210">**Observação:** A participação do convidado depende das configurações de locatário para reunião.</span><span class="sxs-lookup"><span data-stu-id="eb237-210">**Note:** The guest join depends on the tenant settings for meeting.</span></span> <span data-ttu-id="eb237-211">O aplicativo pode ser colocado no lobby esperando para ser admitido por um usuário.</span><span class="sxs-lookup"><span data-stu-id="eb237-211">The application might be put in lobby waiting to be admitted by a user.</span></span> <span data-ttu-id="eb237-212">Isso é definido pela `isInLobby` propriedade</span><span class="sxs-lookup"><span data-stu-id="eb237-212">This is defined by the `isInLobby` property</span></span>

##### <a name="notification---roster"></a><span data-ttu-id="eb237-213">Notificação - lista</span><span class="sxs-lookup"><span data-stu-id="eb237-213">Notification - roster</span></span>

```http
POST https://bot.contoso.com/callback
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/2f1a1100-726f-4705-a071-30fb8f6b568f/participants",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "guest": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "Guest User",
                "id": "d7a3b999-17ac-4bca-9e77-e6a730d2ec2e"
              }
            }
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "sourceId": "10",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": true,
          "id": "05491616-385f-44a8-9974-18cc5f9933c1"
        }
      ]
    }
  ]
}
```
> <span data-ttu-id="eb237-214">**Observação:** O aplicativo não receberá a lista de participantes da reunião até sua entrada no lobby</span><span class="sxs-lookup"><span data-stu-id="eb237-214">**Note:** The application will not receive the roster for participants in the meeting until its admitted from lobby</span></span>

### <a name="example-9-create-peer-to-peer-pstn-call-with-service-hosted-media"></a><span data-ttu-id="eb237-215">Exemplo 9: Criar chamada PSTN ponto a ponto com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="eb237-215">Example 9: Create peer-to-peer PSTN call with service hosted media</span></span>

> <span data-ttu-id="eb237-216">**Observação:** Essa chamada requer o Calls.Initiate. Todas as permissões.</span><span class="sxs-lookup"><span data-stu-id="eb237-216">**Note:** This call requires the Calls.Initiate.All permission.</span></span>

<span data-ttu-id="eb237-217">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="eb237-217">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="eb237-218">Para obter detalhes, [consulte Atribuir um número de telefone ao seu bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span><span class="sxs-lookup"><span data-stu-id="eb237-218">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="eb237-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb237-219">Request</span></span>
<span data-ttu-id="eb237-220">O exemplo a seguir mostra a solicitação para fazer uma chamada ponto a ponto entre o bot e um número PSTN.</span><span class="sxs-lookup"><span data-stu-id="eb237-220">The following example shows the request to make a peer-to-peer call between the bot and a PSTN number.</span></span> <span data-ttu-id="eb237-221">Neste exemplo, a mídia é hospedada pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="eb237-221">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="eb237-222">Os valores de token de autorização, URL de retorno de chamada, ID do aplicativo, nome do aplicativo, ID de usuário, nome de usuário e ID de locatário devem ser substituídos por valores reais para fazer o exemplo funcionar.</span><span class="sxs-lookup"><span data-stu-id="eb237-222">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "applicationInstance": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
    },
    "countryCode": null,
    "endpointType": null,
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig"
  }
}
```

#### <a name="response"></a><span data-ttu-id="eb237-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb237-223">Response</span></span>

> <span data-ttu-id="eb237-224">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="eb237-224">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "applicationInstance": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
    },
    "countryCode": null,
    "endpointType": null,
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      },
      "endpointType": null,
      "region": null,
      "replacesCallId": null,
      "languageId": null
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "activeModalities": [],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "routingPolicies": [],
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#app/calls/$entity",
  "subject": null,
  "terminationReason": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

### <a name="example-10-create-peer-to-peer-pstn-call-with-application-hosted-media"></a><span data-ttu-id="eb237-225">Exemplo 10: Criar chamada PSTN ponto a ponto com mídia hospedada por aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb237-225">Example 10: Create peer-to-peer PSTN call with application hosted media</span></span>

> <span data-ttu-id="eb237-226">**Observação**: este exemplo requer Calls.Initiate. Permissões All e Calls.AccessMedia.All.</span><span class="sxs-lookup"><span data-stu-id="eb237-226">**Note**: This example requires Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

<span data-ttu-id="eb237-227">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="eb237-227">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="eb237-228">Para obter detalhes, [consulte Atribuir um número de telefone ao seu bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span><span class="sxs-lookup"><span data-stu-id="eb237-228">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="eb237-229">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb237-229">Request</span></span>
<span data-ttu-id="eb237-230">O exemplo a seguir mostra uma solicitação para fazer uma chamada ponto a ponto entre o bot e um número PSTN.</span><span class="sxs-lookup"><span data-stu-id="eb237-230">The following example shows a request to make a peer-to-peer call between the bot and a PSTN number.</span></span> <span data-ttu-id="eb237-231">Neste exemplo, a mídia é hospedada localmente pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eb237-231">In this example, the media is hosted locally by the application.</span></span> <span data-ttu-id="eb237-232">Substitua os valores para token de autorização, URL de retorno de chamada, ID do aplicativo, nome do aplicativo, ID de usuário, nome de usuário e ID de locatário para fazer o exemplo funcionar.</span><span class="sxs-lookup"><span data-stu-id="eb237-232">Replace the values for authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID to make the example work.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "applicationInstance": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
    },
    "countryCode": null,
    "endpointType": null,
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>"
  }
}
```

#### <a name="response"></a><span data-ttu-id="eb237-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb237-233">Response</span></span>

> <span data-ttu-id="eb237-234">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="eb237-234">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "applicationInstance": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
    },
    "countryCode": null,
    "endpointType": null,
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      },
      "endpointType": null,
      "region": null,
      "replacesCallId": null,
      "languageId": null
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "activeModalities": [],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>",
  },
  "routingPolicies": [],
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#app/calls/$entity",
  "subject": null,
  "terminationReason": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
