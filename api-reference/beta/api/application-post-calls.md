---
title: Criar chamada
description: Criar uma nova chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 28496a8ed236c3dc5ef43b5a592caf953e8b2d6c
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791139"
---
# <a name="create-call"></a><span data-ttu-id="d56b8-103">Criar chamada</span><span class="sxs-lookup"><span data-stu-id="d56b8-103">Create call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d56b8-104">Criar [chamada](../resources/call.md) permite que o bot crie uma nova chamada de saída ou ingresse em uma reunião existente.</span><span class="sxs-lookup"><span data-stu-id="d56b8-104">Create [call](../resources/call.md) enables your bot to create a new outgoing call or join an existing meeting.</span></span> <span data-ttu-id="d56b8-105">Você precisará [registrar o bot de chamada](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) e passar pela lista de permissões necessárias, conforme mencionado abaixo.</span><span class="sxs-lookup"><span data-stu-id="d56b8-105">You will need to [register the calling bot](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) and go through the list of permissions needed as mentioned below.</span></span>


## <a name="permissions"></a><span data-ttu-id="d56b8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d56b8-106">Permissions</span></span>
<span data-ttu-id="d56b8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span><span class="sxs-lookup"><span data-stu-id="d56b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span></span>

| <span data-ttu-id="d56b8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d56b8-109">Permission type</span></span>                        | <span data-ttu-id="d56b8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d56b8-110">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="d56b8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d56b8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d56b8-112">Não suportado</span><span class="sxs-lookup"><span data-stu-id="d56b8-112">Not Supported</span></span>                                                                           |
| <span data-ttu-id="d56b8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d56b8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d56b8-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="d56b8-114">Not Supported</span></span>                                                                           |
| <span data-ttu-id="d56b8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d56b8-115">Application</span></span>                            | <span data-ttu-id="d56b8-116">Calls. JoinGroupCallsasGuest. All, calls. JoinGroupCalls. All, calls. initiate. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="d56b8-116">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="d56b8-117">**Observação:** Além disso, para uma chamada com mídia hospedada por aplicativo, você precisará da permissão calls. AccessMedia. All.</span><span class="sxs-lookup"><span data-stu-id="d56b8-117">**Note:** In addition, for a call with app hosted media, you need the Calls.AccessMedia.All permission.</span></span>

## <a name="http-request"></a><span data-ttu-id="d56b8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d56b8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
```

## <a name="request-headers"></a><span data-ttu-id="d56b8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d56b8-119">Request headers</span></span>
| <span data-ttu-id="d56b8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d56b8-120">Name</span></span>          | <span data-ttu-id="d56b8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d56b8-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d56b8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d56b8-122">Authorization</span></span> | <span data-ttu-id="d56b8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d56b8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d56b8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d56b8-125">Request body</span></span>
<span data-ttu-id="d56b8-126">No corpo da solicitação, forneça uma representação JSON de um objeto [Call](../resources/call.md) .</span><span class="sxs-lookup"><span data-stu-id="d56b8-126">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

> <span data-ttu-id="d56b8-127">**Observação:** Propriedades marcadas `Server generated` como são ignoradas `POST` quando `app/calls`o processamento é ativado.</span><span class="sxs-lookup"><span data-stu-id="d56b8-127">**Note:** Properties marked as `Server generated` are ignored when processing `POST` on `app/calls`.</span></span>

## <a name="response"></a><span data-ttu-id="d56b8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d56b8-128">Response</span></span>
<span data-ttu-id="d56b8-129">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [Call](../resources/call.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d56b8-129">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d56b8-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d56b8-130">Examples</span></span>

### <a name="create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="d56b8-131">Criar uma chamada VOIP ponto a ponto com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="d56b8-131">Create peer to peer VOIP call with service hosted media</span></span>

> <span data-ttu-id="d56b8-132">**Observação:** Essa chamada precisa da permissão calls. initiate. All.</span><span class="sxs-lookup"><span data-stu-id="d56b8-132">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="d56b8-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d56b8-133">Request</span></span>
<span data-ttu-id="d56b8-134">O exemplo a seguir mostra a solicitação que faz uma chamada ponto a ponto entre o bot e o usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="d56b8-134">The following example shows the request which makes a peer to peer call between the bot and the specified user.</span></span> <span data-ttu-id="d56b8-135">Neste exemplo, a mídia é hospedada pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="d56b8-135">In this example the media is hosted by the service.</span></span> <span data-ttu-id="d56b8-136">Os valores de token de autorização, URL de retorno de chamada, ID de aplicativo, nome de aplicativo, ID de usuário, nome de usuário e ID de locatário devem ser substituídos por valores reais para que o exemplo funcione.</span><span class="sxs-lookup"><span data-stu-id="d56b8-136">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d56b8-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d56b8-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-from-application"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "targets": [
    {
      "@odata.type": "#microsoft.graph.participantInfo",
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
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d56b8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d56b8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d56b8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d56b8-139">Response</span></span>

> <span data-ttu-id="d56b8-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d56b8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/app/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json


{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6",
      }
    },
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.participantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "John",
          "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      },
      "region": null,
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
  "meetingCapability": null,
  "toneInfo": null
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="d56b8-142">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="d56b8-142">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/2e1a0b00-2db4-4022-9570-243709c565ab",
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
##### <a name="notification---established"></a><span data-ttu-id="d56b8-143">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="d56b8-143">Notification - established</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/2e1a0b00-b3c5-4b0f-99b3-c133bc1e6116",
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

### <a name="create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="d56b8-144">Criar uma chamada VOIP ponto a ponto com mídia hospedada pelo aplicativo</span><span class="sxs-lookup"><span data-stu-id="d56b8-144">Create peer to peer VOIP call with application hosted media</span></span>

> <span data-ttu-id="d56b8-145">Observação: precisa de calls. initiate. All e calls. AccessMedia. All.</span><span class="sxs-lookup"><span data-stu-id="d56b8-145">Note: Needs Calls.Initiate.All and Calls.AccessMedia.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="d56b8-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d56b8-146">Request</span></span>
<span data-ttu-id="d56b8-147">O exemplo a seguir mostra a solicitação que faz uma chamada ponto a ponto entre o bot e o usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="d56b8-147">The following example shows the request which makes a peer to peer call between the bot and the specified user.</span></span> <span data-ttu-id="d56b8-148">Neste exemplo, a mídia é hospedada localmente pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d56b8-148">In this example the media is hosted locally by the application.</span></span> <span data-ttu-id="d56b8-149">Os valores de token de autorização, URL de retorno de chamada, ID de aplicativo, nome de aplicativo, ID de usuário, nome de usuário e ID de locatário devem ser substituídos por valores reais para que o exemplo funcione.</span><span class="sxs-lookup"><span data-stu-id="d56b8-149">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "targets": [
    {
      "@odata.type": "#microsoft.graph.participantInfo",
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
    "blob": "<Media Session Configuration>",
  }
}
```
<span data-ttu-id="d56b8-150">`<Media Session Configuration>`é a configuração de sessão de mídia serializada que contém as informações de sessão da pilha de mídia.</span><span class="sxs-lookup"><span data-stu-id="d56b8-150">`<Media Session Configuration>` is the serialized media session configuration which contains the session information of the media stack.</span></span> <span data-ttu-id="d56b8-151">Informações específicas sobre áudio, vídeo, VBSS ssession informações devem ser passadas aqui.</span><span class="sxs-lookup"><span data-stu-id="d56b8-151">Specific information about audio, video, VBSS ssession information should be passed here.</span></span>

<span data-ttu-id="d56b8-152">Exemplo de blob de sessão de mídia de áudio é mostrado abaixo</span><span class="sxs-lookup"><span data-stu-id="d56b8-152">Sample audio media session blob is shown below</span></span>
```json
{\"mpUri\":\"net.tcp://bot.contoso.com:18732/MediaProcessor\",\"audioRenderContexts\":[\"14778cc4-f54c-43c7-989f-9092e34ef784\"],\"videoRenderContexts\":[],\"audioSourceContexts\":[\"a5dcfc9b-5a54-48ef-86f5-1fdd8508741a\"],\"videoSourceContexts\":[],\"dataRenderContexts\":null,\"dataSourceContexts\":null,\"supportedAudioFormat\":\"Pcm16K\",\"videoSinkEncodingFormats\":[],\"mpMediaSessionId\":\"2379cf46-acf3-4fef-a914-be9627075320\",\"regionAffinity\":null,\"skypeMediaBotsVersion\":\"1.11.1.0086\",\"mediaStackVersion\":\"2018.53.1.1\",\"mpVersion\":\"7.2.0.3881\",\"callId\":\"1b69b141-7f1a-4033-9c34-202737190a20\"}
```

><span data-ttu-id="d56b8-153">**Observação:** Para chamadas ponto a ponto, as notificações esperadas são apenas para alterações de estado de chamada.</span><span class="sxs-lookup"><span data-stu-id="d56b8-153">**Note:** For peer to peer calls, the expected notifications are for call state changes only.</span></span>

### <a name="join-scheduled-meeting-with-service-hosted-media"></a><span data-ttu-id="d56b8-154">Ingressar na reunião agendada com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="d56b8-154">Join scheduled meeting with service hosted media</span></span>
<span data-ttu-id="d56b8-155">Para participar da reunião agendada, precisaremos obter a ID do thread, a ID da mensagem, a ID do organizador e a ID do locatário em que a reunião está agendada.</span><span class="sxs-lookup"><span data-stu-id="d56b8-155">To join the scheduled meeting we will need to get the thread id, message id, organizer id and the tenant id in which the meeting is scheduled.</span></span>
<span data-ttu-id="d56b8-156">Essas informações podem ser obtidas na [API obter reuniões online](../api/onlinemeeting-get.md).</span><span class="sxs-lookup"><span data-stu-id="d56b8-156">This information can be obtained from [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="d56b8-157">Os valores do token de autorização, a URL de retorno de chamada, a ID do aplicativo, o nome do aplicativo, a ID do usuário, o nome do usuário e a ID do locatário devem ser substituídos juntamente com os detalhes obtidos da [API obter reuniões online](../api/onlinemeeting-get.md) com valores reais para fazer com que o exemplo funcione.</span><span class="sxs-lookup"><span data-stu-id="d56b8-157">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>
> <span data-ttu-id="d56b8-158">**Observação:** Este exemplo precisa da `Calls.JoinGroupCalls.All` permissão.</span><span class="sxs-lookup"><span data-stu-id="d56b8-158">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="d56b8-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d56b8-159">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
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
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  }
}
```
##### <a name="response"></a><span data-ttu-id="d56b8-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="d56b8-160">Response</span></span>

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/app/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "truncated": "true",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6",
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

##### <a name="notification---establishing"></a><span data-ttu-id="d56b8-161">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="d56b8-161">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92",
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
##### <a name="notification---established"></a><span data-ttu-id="d56b8-162">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="d56b8-162">Notification - established</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92",
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
##### <a name="notification---roster"></a><span data-ttu-id="d56b8-163">Lista de notificação</span><span class="sxs-lookup"><span data-stu-id="d56b8-163">Notification - Roster</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92/participants",
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

><span data-ttu-id="d56b8-164">**Observação:** Para entrar em cenários de reunião distantes de notificações de estado de chamada, recebemos notificações de lista.</span><span class="sxs-lookup"><span data-stu-id="d56b8-164">**Note:** For join meeting scenarios apart from call state notifications, we receive roster notifications.</span></span>

### <a name="join-scheduled-meeting-with-app-hosted-media"></a><span data-ttu-id="d56b8-165">Ingressar na reunião agendada com mídia hospedada por aplicativo</span><span class="sxs-lookup"><span data-stu-id="d56b8-165">Join scheduled meeting with app hosted media</span></span>
<span data-ttu-id="d56b8-166">Para ingressar na reunião com a mídia hospedada por aplicativo, atualize a configuração de mídia com o [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) , conforme mostrado abaixo, no exemplo fornecido acima.</span><span class="sxs-lookup"><span data-stu-id="d56b8-166">To join the meeting with application hosted media update the media config with the [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) as shown below, In the sample provided above.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>
```
<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
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


### <a name="join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="d56b8-167">Reunião de canal de ingresso com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="d56b8-167">Join channel meeting with service hosted media</span></span>
<span data-ttu-id="d56b8-168">A reunião dentro de um canal requer detalhes específicos, como ID do thread, MessageId e detalhes do organizador que podem ser obtidos usando a [API de reuniões online](../api/onlinemeeting-get.md).</span><span class="sxs-lookup"><span data-stu-id="d56b8-168">Meeting inside a channel requires specific details like thread id, messageid, and organizer details that can be obtained using the [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="d56b8-169">Os valores do token de autorização, a URL de retorno de chamada, a ID do aplicativo, o nome do aplicativo, a ID do usuário, o nome do usuário e a ID do locatário devem ser substituídos juntamente com os detalhes obtidos da [API obter reuniões online](../api/onlinemeeting-get.md) com valores reais para fazer com que o exemplo funcione.</span><span class="sxs-lookup"><span data-stu-id="d56b8-169">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>

> <span data-ttu-id="d56b8-170">**Observação:** Este exemplo precisa da `Calls.JoinGroupCalls.All` permissão.</span><span class="sxs-lookup"><span data-stu-id="d56b8-170">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="d56b8-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d56b8-171">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
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

### <a name="join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="d56b8-172">Ingressar na reunião de canal como um convidado com mídia de serviço hospedado</span><span class="sxs-lookup"><span data-stu-id="d56b8-172">Join channel meeting as a guest with service hosted media</span></span>
<span data-ttu-id="d56b8-173">Para ingressar em uma reunião de canal como convidado, você precisará criar uma [identidade](../resources/identityset.md) de convidado e adicioná-la como fonte de chamada na solicitação de reunião de ingresso.</span><span class="sxs-lookup"><span data-stu-id="d56b8-173">For joining a channel meeting as a guest you will need to create a guest [identity](../resources/identityset.md) and add it as the call source in the join meeting request.</span></span>
<span data-ttu-id="d56b8-174">O nome para exibição é o nome que você deseja exibir na reunião para sua identidade de convidado.</span><span class="sxs-lookup"><span data-stu-id="d56b8-174">The display name is the name you want to be displayed in the meeting for your guest identity.</span></span> <span data-ttu-id="d56b8-175">A ID pode ser uma ID exclusiva que identifica a identidade de convidado.</span><span class="sxs-lookup"><span data-stu-id="d56b8-175">The id may be a unique id identifying the guest identity.</span></span>

> <span data-ttu-id="d56b8-176">**Observação:** Este exemplo precisa da `Calls.JoinGroupCallsAsGuest.All` permissão.</span><span class="sxs-lookup"><span data-stu-id="d56b8-176">**Note:** This example needs the `Calls.JoinGroupCallsAsGuest.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="d56b8-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d56b8-177">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
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
> <span data-ttu-id="d56b8-178">**Observação:** A associação de convidados depende das configurações de locatário para a reunião.</span><span class="sxs-lookup"><span data-stu-id="d56b8-178">**Note:** The guest join depends on the tenant settings for meeting.</span></span> <span data-ttu-id="d56b8-179">O aplicativo pode ser colocado no lobby esperando ser admitido por um usuário.</span><span class="sxs-lookup"><span data-stu-id="d56b8-179">The application might be put in lobby waiting to be admitted by a user.</span></span> <span data-ttu-id="d56b8-180">Isso é definido pela `isInLobby` Propriedade</span><span class="sxs-lookup"><span data-stu-id="d56b8-180">This is defined by the `isInLobby` property</span></span>

##### <a name="notification---roster"></a><span data-ttu-id="d56b8-181">Lista de notificação</span><span class="sxs-lookup"><span data-stu-id="d56b8-181">Notification - Roster</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/2f1a1100-726f-4705-a071-30fb8f6b568f/participants",
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
> <span data-ttu-id="d56b8-182">**Observação:** O aplicativo não receberá a lista de participantes da reunião até seu admitiu no lobby</span><span class="sxs-lookup"><span data-stu-id="d56b8-182">**Note:** The application will not receive the roster for participants in the meeting until its admitted from lobby</span></span>
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
