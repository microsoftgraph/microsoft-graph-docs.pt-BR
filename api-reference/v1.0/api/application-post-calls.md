---
title: Criar chamada
description: Criar uma nova chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a9631f6b8dfb8335d7747e5f6531cb1942417d6d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865752"
---
# <a name="create-call"></a><span data-ttu-id="f9c49-103">Criar chamada</span><span class="sxs-lookup"><span data-stu-id="f9c49-103">Create call</span></span>

<span data-ttu-id="f9c49-104">Criar [chamada](../resources/call.md) permite que o bot crie uma nova chamada ponto a ponto ou de saída de grupo, ou ingresse em uma reunião existente.</span><span class="sxs-lookup"><span data-stu-id="f9c49-104">Create [call](../resources/call.md) enables your bot to create a new outgoing peer-to-peer or group call, or join an existing meeting.</span></span> <span data-ttu-id="f9c49-105">Você precisará [registrar o bot de chamada](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) e passar pela lista de permissões necessárias, conforme mencionado abaixo.</span><span class="sxs-lookup"><span data-stu-id="f9c49-105">You will need to [register the calling bot](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) and go through the list of permissions needed as mentioned below.</span></span>

> <span data-ttu-id="f9c49-106">**Observação:** No momento, só há suporte para chamadas VoIP.</span><span class="sxs-lookup"><span data-stu-id="f9c49-106">**Note:** Currently, only VoIP calls are supported.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f9c49-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9c49-107">Permissions</span></span>

<span data-ttu-id="f9c49-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span><span class="sxs-lookup"><span data-stu-id="f9c49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span></span>

| <span data-ttu-id="f9c49-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9c49-110">Permission type</span></span>                        | <span data-ttu-id="f9c49-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9c49-111">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="f9c49-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9c49-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9c49-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="f9c49-113">Not Supported</span></span>                                                                           |
| <span data-ttu-id="f9c49-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9c49-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9c49-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="f9c49-115">Not Supported</span></span>                                                                           |
| <span data-ttu-id="f9c49-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9c49-116">Application</span></span>                            | <span data-ttu-id="f9c49-117">Calls. JoinGroupCallsasGuest. All, calls. JoinGroupCalls. All, calls. initiate. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="f9c49-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="f9c49-118">**Observação:** Para uma chamada com mídia hospedada em aplicativos, você precisará da permissão calls. AccessMedia. All além de uma das permissões listadas na tabela acima.</span><span class="sxs-lookup"><span data-stu-id="f9c49-118">**Note:** For a call with app-hosted media, you need the Calls.AccessMedia.All permission in addition to one of the permissions listed in the table above.</span></span>

## <a name="http-request"></a><span data-ttu-id="f9c49-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9c49-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls
```

## <a name="request-headers"></a><span data-ttu-id="f9c49-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9c49-120">Request headers</span></span>
| <span data-ttu-id="f9c49-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f9c49-121">Name</span></span>          | <span data-ttu-id="f9c49-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9c49-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f9c49-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9c49-123">Authorization</span></span> | <span data-ttu-id="f9c49-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9c49-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9c49-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="f9c49-126">Content-type</span></span>  | <span data-ttu-id="f9c49-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9c49-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9c49-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9c49-129">Request body</span></span>
<span data-ttu-id="f9c49-130">No corpo da solicitação, forneça uma representação JSON de um objeto [Call](../resources/call.md) .</span><span class="sxs-lookup"><span data-stu-id="f9c49-130">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f9c49-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9c49-131">Response</span></span>
<span data-ttu-id="f9c49-132">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [Call](../resources/call.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9c49-132">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f9c49-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f9c49-133">Examples</span></span>

### <a name="example-1-create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="f9c49-134">Exemplo 1: criar uma chamada VoIP ponto a ponto com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="f9c49-134">Example 1: Create peer-to-peer VoIP call with service hosted media</span></span>

> <span data-ttu-id="f9c49-135">**Observação:** Essa chamada precisa da permissão calls. initiate. All.</span><span class="sxs-lookup"><span data-stu-id="f9c49-135">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="f9c49-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9c49-136">Request</span></span>
<span data-ttu-id="f9c49-137">O exemplo a seguir mostra a solicitação que faz uma chamada ponto a ponto entre o bot e o usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="f9c49-137">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="f9c49-138">Neste exemplo, a mídia é hospedada pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="f9c49-138">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="f9c49-139">Os valores do token de autorização, a URL de retorno de chamada, a ID do aplicativo, o nome do aplicativo, a ID do usuário, o nome do usuário e a ID do locatário devem ser substituídos por valores reais para que o exemplo funcione.</span><span class="sxs-lookup"><span data-stu-id="f9c49-139">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f9c49-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9c49-140">HTTP</span></span>](#tab/http)
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
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9c49-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9c49-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-service-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="f9c49-142">C#</span><span class="sxs-lookup"><span data-stu-id="f9c49-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-service-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f9c49-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9c49-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-service-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f9c49-144">Java</span><span class="sxs-lookup"><span data-stu-id="f9c49-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-service-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f9c49-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9c49-145">Response</span></span>

> <span data-ttu-id="f9c49-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f9c49-146">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
  "toneInfo": null
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="f9c49-147">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="f9c49-147">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="f9c49-148">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="f9c49-148">Notification - established</span></span>

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

### <a name="example-2-create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="f9c49-149">Exemplo 2: criar uma chamada VoIP ponto a ponto com mídia hospedada no aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9c49-149">Example 2: Create peer-to-peer VoIP call with application hosted media</span></span>

> <span data-ttu-id="f9c49-150">**Observação**: Este exemplo precisa de calls. initiate. All e calls. AccessMedia. All.</span><span class="sxs-lookup"><span data-stu-id="f9c49-150">**Note**: This example needs Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="f9c49-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9c49-151">Request</span></span>
<span data-ttu-id="f9c49-152">O exemplo a seguir mostra a solicitação que faz uma chamada ponto a ponto entre o bot e o usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="f9c49-152">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="f9c49-153">Neste exemplo, a mídia é hospedada localmente pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f9c49-153">In this example the media is hosted locally by the application.</span></span> <span data-ttu-id="f9c49-154">Os valores de token de autorização, URL de retorno de chamada, ID de aplicativo, nome de aplicativo, ID de usuário, nome de usuário e ID de locatário devem ser substituídos por valores reais para que o exemplo funcione.</span><span class="sxs-lookup"><span data-stu-id="f9c49-154">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f9c49-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9c49-155">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f9c49-156">C#</span><span class="sxs-lookup"><span data-stu-id="f9c49-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9c49-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9c49-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f9c49-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9c49-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f9c49-159">Java</span><span class="sxs-lookup"><span data-stu-id="f9c49-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

><span data-ttu-id="f9c49-160">**Observação:** Para chamadas ponto a ponto, as notificações esperadas são apenas para alterações de estado de chamada.</span><span class="sxs-lookup"><span data-stu-id="f9c49-160">**Note:** For peer-to-peer calls, the expected notifications are for call state changes only.</span></span>

##### <a name="response"></a><span data-ttu-id="f9c49-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9c49-161">Response</span></span>

> <span data-ttu-id="f9c49-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9c49-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "toneInfo": null
}
```

### <a name="example-3-create-a-group-call-with-service-hosted-media"></a><span data-ttu-id="f9c49-164">Exemplo 3: criar uma chamada de grupo com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="f9c49-164">Example 3: Create a group call with service hosted media</span></span>

<span data-ttu-id="f9c49-165">Isso oferece suporte a até 5 usuários de VoIP.</span><span class="sxs-lookup"><span data-stu-id="f9c49-165">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="f9c49-166">O exemplo mostra como criar uma chamada de grupo com dois usuários de VoIP.</span><span class="sxs-lookup"><span data-stu-id="f9c49-166">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="f9c49-167">**Observação:** Esta chamada de exemplo precisa `Calls.InitiateGroupCalls.All` da permissão.</span><span class="sxs-lookup"><span data-stu-id="f9c49-167">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="f9c49-168">A chamada de grupo criada não dá suporte a chat ou gravação.</span><span class="sxs-lookup"><span data-stu-id="f9c49-168">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="f9c49-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9c49-169">Request</span></span>

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

### <a name="example-4-create-a-group-call-with-application-hosted-media"></a><span data-ttu-id="f9c49-170">Exemplo 4: criar uma chamada de grupo com mídia hospedada por aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9c49-170">Example 4: Create a group call with application hosted media</span></span>

<span data-ttu-id="f9c49-171">Isso oferece suporte a até 5 usuários de VoIP.</span><span class="sxs-lookup"><span data-stu-id="f9c49-171">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="f9c49-172">O exemplo mostra como criar uma chamada de grupo com dois usuários de VoIP.</span><span class="sxs-lookup"><span data-stu-id="f9c49-172">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="f9c49-173">**Observação:** Esta chamada de exemplo precisa `Calls.InitiateGroupCalls.All` da permissão.</span><span class="sxs-lookup"><span data-stu-id="f9c49-173">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="f9c49-174">A chamada de grupo criada não dá suporte a chat ou gravação.</span><span class="sxs-lookup"><span data-stu-id="f9c49-174">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="f9c49-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9c49-175">Request</span></span>

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

### <a name="example-5-join-scheduled-meeting-with-service-hosted-media"></a><span data-ttu-id="f9c49-176">Exemplo 5: ingressar na reunião agendada com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="f9c49-176">Example 5: Join scheduled meeting with service hosted media</span></span>
<span data-ttu-id="f9c49-177">Para participar da reunião agendada, precisaremos obter a ID do thread, a ID da mensagem, a ID do organizador e a ID do locatário em que a reunião está agendada.</span><span class="sxs-lookup"><span data-stu-id="f9c49-177">To join the scheduled meeting we will need to get the thread id, message id, organizer id and the tenant id in which the meeting is scheduled.</span></span>
<span data-ttu-id="f9c49-178">Essas informações podem ser obtidas na [API de reuniões online](../api/onlinemeeting-get.md) (somente em reuniões do VTC).</span><span class="sxs-lookup"><span data-stu-id="f9c49-178">This information can be obtained from the [Get Online Meetings API](../api/onlinemeeting-get.md) (VTC-based meetings only).</span></span>

<span data-ttu-id="f9c49-179">Os valores do token de autorização, a URL de retorno de chamada, a ID do aplicativo, o nome do aplicativo, a ID do usuário, o nome do usuário e a ID do locatário devem ser substituídos juntamente com os detalhes obtidos da [API de reunião online](../api/onlinemeeting-get.md) (somente em reuniões do VTC) com valores reais para que o exemplo funcione.</span><span class="sxs-lookup"><span data-stu-id="f9c49-179">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) (VTC-based meetings only) with actual values to make the example work.</span></span>
> <span data-ttu-id="f9c49-180">**Observação:** Este exemplo precisa da `Calls.JoinGroupCalls.All` permissão.</span><span class="sxs-lookup"><span data-stu-id="f9c49-180">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="f9c49-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9c49-181">Request</span></span>

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
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  }
}
```
##### <a name="response"></a><span data-ttu-id="f9c49-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9c49-182">Response</span></span>

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

##### <a name="notification---establishing"></a><span data-ttu-id="f9c49-183">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="f9c49-183">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="f9c49-184">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="f9c49-184">Notification - established</span></span>

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
##### <a name="notification---roster"></a><span data-ttu-id="f9c49-185">Lista de notificação</span><span class="sxs-lookup"><span data-stu-id="f9c49-185">Notification - roster</span></span>

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

><span data-ttu-id="f9c49-186">**Observação:** Para entrar em cenários de reunião distantes de notificações de estado de chamada, recebemos notificações de lista.</span><span class="sxs-lookup"><span data-stu-id="f9c49-186">**Note:** For join meeting scenarios apart from call state notifications, we receive roster notifications.</span></span>

### <a name="example-6-join-scheduled-meeting-with-application-hosted-media"></a><span data-ttu-id="f9c49-187">Exemplo 6: ingressar na reunião agendada com mídia hospedada de aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9c49-187">Example 6: Join scheduled meeting with application hosted media</span></span>
<span data-ttu-id="f9c49-188">Atualize a configuração de mídia com o [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) , como mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="f9c49-188">Update the media config with the [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) as shown below.</span></span>

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
