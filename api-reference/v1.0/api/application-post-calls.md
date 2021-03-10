---
title: Criar chamada
description: Crie uma nova chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: cf26ec2ebb0cd17e2091ae5292df0069e0649203
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575718"
---
# <a name="create-call"></a><span data-ttu-id="86967-103">Criar chamada</span><span class="sxs-lookup"><span data-stu-id="86967-103">Create call</span></span>

<span data-ttu-id="86967-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86967-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="86967-105">Criar [chamada](../resources/call.md) permite que seu bot crie uma nova chamada ponto a ponto ou grupo de saída ou participe de uma reunião existente.</span><span class="sxs-lookup"><span data-stu-id="86967-105">Create [call](../resources/call.md) enables your bot to create a new outgoing peer-to-peer or group call, or join an existing meeting.</span></span> <span data-ttu-id="86967-106">Você precisará registrar [o bot de chamada](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) e passar pela lista de permissões necessárias, conforme mencionado abaixo.</span><span class="sxs-lookup"><span data-stu-id="86967-106">You will need to [register the calling bot](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) and go through the list of permissions needed as mentioned below.</span></span>

> <span data-ttu-id="86967-107">**Observação:** Atualmente, apenas chamadas VoIP são suportadas.</span><span class="sxs-lookup"><span data-stu-id="86967-107">**Note:** Currently, only VoIP calls are supported.</span></span> 

## <a name="permissions"></a><span data-ttu-id="86967-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="86967-108">Permissions</span></span>

<span data-ttu-id="86967-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span><span class="sxs-lookup"><span data-stu-id="86967-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span></span>

| <span data-ttu-id="86967-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86967-111">Permission type</span></span>                        | <span data-ttu-id="86967-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86967-112">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="86967-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86967-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="86967-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="86967-114">Not Supported</span></span>                                                                           |
| <span data-ttu-id="86967-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86967-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86967-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="86967-116">Not Supported</span></span>                                                                           |
| <span data-ttu-id="86967-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86967-117">Application</span></span>                            | <span data-ttu-id="86967-118">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate. All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="86967-118">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="86967-119">**Observação:** Para uma chamada com mídia hospedada por aplicativo, você precisa da permissão Calls.AccessMedia.All, além de uma das permissões listadas na tabela acima.</span><span class="sxs-lookup"><span data-stu-id="86967-119">**Note:** For a call with app-hosted media, you need the Calls.AccessMedia.All permission in addition to one of the permissions listed in the table above.</span></span>

## <a name="http-request"></a><span data-ttu-id="86967-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86967-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls
```

## <a name="request-headers"></a><span data-ttu-id="86967-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86967-121">Request headers</span></span>
| <span data-ttu-id="86967-122">Nome</span><span class="sxs-lookup"><span data-stu-id="86967-122">Name</span></span>          | <span data-ttu-id="86967-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="86967-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="86967-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="86967-124">Authorization</span></span> | <span data-ttu-id="86967-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86967-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="86967-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="86967-127">Content-type</span></span>  | <span data-ttu-id="86967-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86967-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86967-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86967-130">Request body</span></span>
<span data-ttu-id="86967-131">No corpo da solicitação, fornece uma representação JSON de um [objeto de](../resources/call.md) chamada.</span><span class="sxs-lookup"><span data-stu-id="86967-131">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="86967-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="86967-132">Response</span></span>
<span data-ttu-id="86967-133">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto de](../resources/call.md) chamada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86967-133">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86967-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="86967-134">Examples</span></span>

### <a name="example-1-create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="86967-135">Exemplo 1: Criar chamada VoIP ponto a ponto com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="86967-135">Example 1: Create peer-to-peer VoIP call with service hosted media</span></span>

> <span data-ttu-id="86967-136">**Observação:** Essa chamada precisa da Calls.Initiate. Todas as permissões.</span><span class="sxs-lookup"><span data-stu-id="86967-136">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="86967-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86967-137">Request</span></span>
<span data-ttu-id="86967-138">O exemplo a seguir mostra a solicitação que faz uma chamada ponto a ponto entre o bot e o usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="86967-138">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="86967-139">Neste exemplo, a mídia é hospedada pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="86967-139">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="86967-140">Os valores de token de autorização, URL de retorno de chamada, ID do aplicativo, nome do aplicativo, ID de usuário, nome de usuário e ID de locatário devem ser substituídos por valores reais para fazer o exemplo funcionar.</span><span class="sxs-lookup"><span data-stu-id="86967-140">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="86967-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="86967-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls
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
# <a name="javascript"></a>[<span data-ttu-id="86967-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86967-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-service-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="86967-143">C#</span><span class="sxs-lookup"><span data-stu-id="86967-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-service-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86967-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86967-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-service-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86967-145">Java</span><span class="sxs-lookup"><span data-stu-id="86967-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-service-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="86967-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="86967-146">Response</span></span>

> <span data-ttu-id="86967-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="86967-147">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
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
      "replacesCallId": null,
    }
  ],
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
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#app/calls/$entity",
  "subject": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "toneInfo": null
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="86967-148">Notificação - estabelecimento</span><span class="sxs-lookup"><span data-stu-id="86967-148">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="86967-149">Notificação - estabelecida</span><span class="sxs-lookup"><span data-stu-id="86967-149">Notification - established</span></span>

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
        "id": "2e1a0b00-b3c5-4b0f-99b3-c133bc1e6116"
      }
    }
  ]
}
```

### <a name="example-2-create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="86967-150">Exemplo 2: Criar chamada VoIP ponto a ponto com mídia hospedada por aplicativo</span><span class="sxs-lookup"><span data-stu-id="86967-150">Example 2: Create peer-to-peer VoIP call with application hosted media</span></span>

> <span data-ttu-id="86967-151">**Observação**: este exemplo precisa Calls.Initiate. Permissões All e Calls.AccessMedia.All.</span><span class="sxs-lookup"><span data-stu-id="86967-151">**Note**: This example needs Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="86967-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86967-152">Request</span></span>
<span data-ttu-id="86967-153">O exemplo a seguir mostra a solicitação que faz uma chamada ponto a ponto entre o bot e o usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="86967-153">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="86967-154">Neste exemplo, a mídia é hospedada localmente pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86967-154">In this example the media is hosted locally by the application.</span></span> <span data-ttu-id="86967-155">Os valores de token de autorização, url de retorno de chamada, id do aplicativo, nome do aplicativo, id de usuário, nome de usuário e id de locatário devem ser substituídos por valores reais para fazer o exemplo funcionar.</span><span class="sxs-lookup"><span data-stu-id="86967-155">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="86967-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="86967-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-app-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls
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
# <a name="c"></a>[<span data-ttu-id="86967-157">C#</span><span class="sxs-lookup"><span data-stu-id="86967-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86967-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86967-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86967-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86967-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86967-160">Java</span><span class="sxs-lookup"><span data-stu-id="86967-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

><span data-ttu-id="86967-161">**Observação:** Para chamadas ponto a ponto, as notificações esperadas são apenas para alterações de estado de chamada.</span><span class="sxs-lookup"><span data-stu-id="86967-161">**Note:** For peer-to-peer calls, the expected notifications are for call state changes only.</span></span>

##### <a name="response"></a><span data-ttu-id="86967-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="86967-162">Response</span></span>

> <span data-ttu-id="86967-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86967-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
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
    "blob": "<Media Session Configuration>",
  },
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#app/calls/$entity",
  "subject": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "toneInfo": null
}
```

### <a name="example-3-create-a-group-call-with-service-hosted-media"></a><span data-ttu-id="86967-165">Exemplo 3: Criar uma chamada de grupo com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="86967-165">Example 3: Create a group call with service hosted media</span></span>

<span data-ttu-id="86967-166">Isso dá suporte a até 5 usuários VoIP.</span><span class="sxs-lookup"><span data-stu-id="86967-166">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="86967-167">O exemplo mostra como criar uma chamada de grupo com dois usuários VoIP.</span><span class="sxs-lookup"><span data-stu-id="86967-167">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="86967-168">**Observação:** Esta chamada de exemplo precisa da `Calls.InitiateGroupCalls.All` permissão.</span><span class="sxs-lookup"><span data-stu-id="86967-168">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="86967-169">A chamada de grupo criada não dá suporte a chat ou gravação.</span><span class="sxs-lookup"><span data-stu-id="86967-169">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="86967-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86967-170">Request</span></span>

<!-- {
  "blockType": "example",
  "name": "create-group-call-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls
Content-Type: application/json

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
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
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
  }
}
```

### <a name="example-4-create-a-group-call-with-application-hosted-media"></a><span data-ttu-id="86967-171">Exemplo 4: Criar uma chamada de grupo com mídia hospedada por aplicativo</span><span class="sxs-lookup"><span data-stu-id="86967-171">Example 4: Create a group call with application hosted media</span></span>

<span data-ttu-id="86967-172">Isso dá suporte a até 5 usuários VoIP.</span><span class="sxs-lookup"><span data-stu-id="86967-172">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="86967-173">O exemplo mostra como criar uma chamada de grupo com dois usuários VoIP.</span><span class="sxs-lookup"><span data-stu-id="86967-173">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="86967-174">**Observação:** Esta chamada de exemplo precisa da `Calls.InitiateGroupCalls.All` permissão.</span><span class="sxs-lookup"><span data-stu-id="86967-174">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="86967-175">A chamada de grupo criada não dá suporte a chat ou gravação.</span><span class="sxs-lookup"><span data-stu-id="86967-175">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="86967-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86967-176">Request</span></span>

<!-- {
  "blockType": "example",
  "name": "create-group-call-app-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "direction": "outgoing",
  "subject": "Create a group call with application hosted media",
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
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
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
    "removeFromDefaultAudioGroup": false
  }
}
```

### <a name="example-5-join-scheduled-meeting-with-service-hosted-media"></a><span data-ttu-id="86967-177">Exemplo 5: Participar de reunião agendada com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="86967-177">Example 5: Join scheduled meeting with service hosted media</span></span>
<span data-ttu-id="86967-178">Para participar da reunião agendada, precisamos obter a ID do thread, a ID da mensagem, a ID do organizador e a id do locatário na qual a reunião está agendada.</span><span class="sxs-lookup"><span data-stu-id="86967-178">To join the scheduled meeting we will need to get the thread id, message id, organizer id and the tenant id in which the meeting is scheduled.</span></span>
<span data-ttu-id="86967-179">Essas informações podem ser obtidas da [API Get Online Meetings](../api/onlinemeeting-get.md) (somente reuniões baseadas em VTC).</span><span class="sxs-lookup"><span data-stu-id="86967-179">This information can be obtained from the [Get Online Meetings API](../api/onlinemeeting-get.md) (VTC-based meetings only).</span></span>

<span data-ttu-id="86967-180">Os valores de token de autorização, url de retorno de chamada, id de aplicativo, nome de aplicativo, id de usuário, nome de usuário e id de locatário devem ser substituídos juntamente com os detalhes obtidos da  [API de](../api/onlinemeeting-get.md) Reuniões Get Online (somente reuniões baseadas em VTC) com valores reais para fazer o exemplo funcionar.</span><span class="sxs-lookup"><span data-stu-id="86967-180">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) (VTC-based meetings only) with actual values to make the example work.</span></span>
> <span data-ttu-id="86967-181">**Observação:** Este exemplo precisa da `Calls.JoinGroupCalls.All` permissão.</span><span class="sxs-lookup"><span data-stu-id="86967-181">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="86967-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86967-182">Request</span></span>

<!-- {
  "blockType": "example",
  "name": "join-scheduled-meeting-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls
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
        "displayName": "Bob",
        "tenantId":"86dc81db-c112-4228-9222-63f3esaa1edb"
      }
    },
    "allowConversationWithoutHost": true
  },
  "tenantId":"86dc81db-c112-4228-9222-63f3esaa1edb"
}
```
##### <a name="response"></a><span data-ttu-id="86967-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="86967-183">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": "true",
  "@odata.type": "microsoft.graph.call"
}-->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
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
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  },
  "transcription": null,
  "myParticipantId": "05491616-385f-44a8-9974-18cc5f9933c1",
  "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#app/calls/$entity",
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "subject": null,
  "resultInfo": null,
  "answeredBy": null,
  "toneInfo": null
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="86967-184">Notificação - estabelecimento</span><span class="sxs-lookup"><span data-stu-id="86967-184">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="86967-185">Notificação - estabelecida</span><span class="sxs-lookup"><span data-stu-id="86967-185">Notification - established</span></span>

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
##### <a name="notification---roster"></a><span data-ttu-id="86967-186">Notificação - lista</span><span class="sxs-lookup"><span data-stu-id="86967-186">Notification - roster</span></span>

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

><span data-ttu-id="86967-187">**Observação:** Para participar de cenários de reunião, além das notificações de estado de chamada, recebemos notificações de lista.</span><span class="sxs-lookup"><span data-stu-id="86967-187">**Note:** For join meeting scenarios apart from call state notifications, we receive roster notifications.</span></span>

### <a name="example-6-join-scheduled-meeting-with-application-hosted-media"></a><span data-ttu-id="86967-188">Exemplo 6: Participar de uma reunião agendada com a mídia hospedada pelo aplicativo</span><span class="sxs-lookup"><span data-stu-id="86967-188">Example 6: Join scheduled meeting with application hosted media</span></span>
<span data-ttu-id="86967-189">Atualize a configuração de mídia com [o AppHostedMediaConfig,](../resources/apphostedmediaconfig.md) conforme mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="86967-189">Update the media config with the [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) as shown below.</span></span>

<!-- {
  "blockType": "example",
  "name": "join-scheduled-meeting-app-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig"
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
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  }
}
```

### <a name="example-7-create-peer-to-peer-pstn-call-with-service-hosted-media"></a><span data-ttu-id="86967-190">Exemplo 7: Criar chamada PSTN ponto a ponto com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="86967-190">Example 7: Create peer-to-peer PSTN call with service hosted media</span></span>

> <span data-ttu-id="86967-191">**Observação:** Essa chamada requer o Calls.Initiate. Todas as permissões.</span><span class="sxs-lookup"><span data-stu-id="86967-191">**Note:** This call requires the Calls.Initiate.All permission.</span></span>

<span data-ttu-id="86967-192">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="86967-192">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="86967-193">Para obter detalhes, [consulte Atribuir um número de telefone ao seu bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span><span class="sxs-lookup"><span data-stu-id="86967-193">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="86967-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86967-194">Request</span></span>
<span data-ttu-id="86967-195">O exemplo a seguir mostra a solicitação para fazer uma chamada ponto a ponto entre o bot e um número PSTN.</span><span class="sxs-lookup"><span data-stu-id="86967-195">The following example shows the request to make a peer-to-peer call between the bot and a PSTN number.</span></span> <span data-ttu-id="86967-196">Neste exemplo, a mídia é hospedada pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="86967-196">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="86967-197">Os valores de token de autorização, URL de retorno de chamada, ID do aplicativo, nome do aplicativo, ID de usuário, nome de usuário e ID de locatário devem ser substituídos por valores reais para fazer o exemplo funcionar.</span><span class="sxs-lookup"><span data-stu-id="86967-197">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls
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

#### <a name="response"></a><span data-ttu-id="86967-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="86967-198">Response</span></span>

> <span data-ttu-id="86967-199">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="86967-199">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#app/calls/$entity",
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

### <a name="example-8-create-peer-to-peer-pstn-call-with-application-hosted-media"></a><span data-ttu-id="86967-200">Exemplo 8: Criar chamada PSTN ponto a ponto com a mídia hospedada pelo aplicativo</span><span class="sxs-lookup"><span data-stu-id="86967-200">Example 8: Create peer-to-peer PSTN call with application hosted media</span></span>

> <span data-ttu-id="86967-201">**Observação**: este exemplo requer Calls.Initiate. Permissões All e Calls.AccessMedia.All.</span><span class="sxs-lookup"><span data-stu-id="86967-201">**Note**: This example requires Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

<span data-ttu-id="86967-202">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="86967-202">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="86967-203">Para obter detalhes, [consulte Atribuir um número de telefone ao seu bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span><span class="sxs-lookup"><span data-stu-id="86967-203">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="86967-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86967-204">Request</span></span>
<span data-ttu-id="86967-205">O exemplo a seguir mostra uma solicitação para fazer uma chamada ponto a ponto entre o bot e um número PSTN.</span><span class="sxs-lookup"><span data-stu-id="86967-205">The following example shows a request to make a peer-to-peer call between the bot and a PSTN number.</span></span> <span data-ttu-id="86967-206">Neste exemplo, a mídia é hospedada localmente pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86967-206">In this example, the media is hosted locally by the application.</span></span> <span data-ttu-id="86967-207">Substitua os valores para token de autorização, URL de retorno de chamada, ID do aplicativo, nome do aplicativo, ID de usuário, nome de usuário e ID de locatário para fazer o exemplo funcionar.</span><span class="sxs-lookup"><span data-stu-id="86967-207">Replace the values for authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID to make the example work.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls
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

#### <a name="response"></a><span data-ttu-id="86967-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="86967-208">Response</span></span>

> <span data-ttu-id="86967-209">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="86967-209">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#app/calls/$entity",
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
