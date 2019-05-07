---
title: Criar chamada
description: Criar uma nova chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 25e716c25ee8d06f5564b8ac6b4e3f6476f0ce84
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636454"
---
# <a name="create-call"></a><span data-ttu-id="fb6a5-103">Criar chamada</span><span class="sxs-lookup"><span data-stu-id="fb6a5-103">Create call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb6a5-104">Criar uma nova chamada.</span><span class="sxs-lookup"><span data-stu-id="fb6a5-104">Create a new call.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb6a5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb6a5-105">Permissions</span></span>
<span data-ttu-id="fb6a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb6a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fb6a5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb6a5-108">Permission type</span></span>                        | <span data-ttu-id="fb6a5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb6a5-109">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="fb6a5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb6a5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb6a5-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="fb6a5-111">Not Supported</span></span>                                                                           |
| <span data-ttu-id="fb6a5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb6a5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb6a5-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="fb6a5-113">Not Supported</span></span>                                                                           |
| <span data-ttu-id="fb6a5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb6a5-114">Application</span></span>                            | <span data-ttu-id="fb6a5-115">Calls. JoinGroupCallsasGuest. All, calls. JoinGroupCalls. All, calls. initiate. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="fb6a5-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="fb6a5-116">**Observação:** Para uma chamada com mídia hospedada por aplicativo, você precisará da permissão calls. AccessMedia. All com uma das permissões listadas na tabela anterior.</span><span class="sxs-lookup"><span data-stu-id="fb6a5-116">**Note:** For a call with app hosted media, you need the Calls.AccessMedia.All permission with one of the permissions listed in the previous table.</span></span>

## <a name="http-request"></a><span data-ttu-id="fb6a5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb6a5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
POST /applications/{id}/calls
```

## <a name="request-headers"></a><span data-ttu-id="fb6a5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb6a5-118">Request headers</span></span>
| <span data-ttu-id="fb6a5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fb6a5-119">Name</span></span>          | <span data-ttu-id="fb6a5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb6a5-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fb6a5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb6a5-121">Authorization</span></span> | <span data-ttu-id="fb6a5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb6a5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb6a5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb6a5-124">Request body</span></span>
<span data-ttu-id="fb6a5-125">No corpo da solicitação, forneça uma representação JSON de um objeto [Call](../resources/call.md) .</span><span class="sxs-lookup"><span data-stu-id="fb6a5-125">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

> <span data-ttu-id="fb6a5-126">**Observação:** Propriedades marcadas `Server generated` como são ignoradas `POST` quando `app/calls`o processamento é ativado.</span><span class="sxs-lookup"><span data-stu-id="fb6a5-126">**Note:** Properties marked as `Server generated` are ignored when processing `POST` on `app/calls`.</span></span>

## <a name="response"></a><span data-ttu-id="fb6a5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb6a5-127">Response</span></span>
<span data-ttu-id="fb6a5-128">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [Call](../resources/call.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb6a5-128">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fb6a5-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fb6a5-129">Examples</span></span>

### <a name="create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="fb6a5-130">Criar uma chamada VOIP ponto a ponto com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="fb6a5-130">Create peer to peer VOIP call with service hosted media</span></span>

> <span data-ttu-id="fb6a5-131">**Observação:** Essa chamada precisa da permissão calls. initiate. All.</span><span class="sxs-lookup"><span data-stu-id="fb6a5-131">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="fb6a5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb6a5-132">Request</span></span>
<span data-ttu-id="fb6a5-133">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb6a5-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-call-from-application"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json

{
  "callbackUri": "https://bot.contoso.com/api/calls",
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
  },
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "subject": "Test Call",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      }
    }
  ],
  "tenantId": "tenantId-value"
}
```

##### <a name="response"></a><span data-ttu-id="fb6a5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb6a5-134">Response</span></span>

> <span data-ttu-id="fb6a5-p103">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb6a5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json


{
  "id": "57DAB8B1894C409AB240BD8BEAE78896",
  "callbackUri": "https://bot.contoso.com/api/calls",
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
  },
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "subject": "Test Call",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      }
    }
  ],
  "tenantId": "tenantId-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fb6a5-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="fb6a5-137">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fb6a5-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb6a5-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-call-from-application-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="notification---establishing"></a><span data-ttu-id="fb6a5-139">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="fb6a5-139">Notification - establishing</span></span>

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
        "state": "establishing",
        "direction": "outgoing"
      }
    }
  ]
}
```
##### <a name="notification---established"></a><span data-ttu-id="fb6a5-140">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="fb6a5-140">Notification - established</span></span>

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

### <a name="create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="fb6a5-141">Criar uma chamada VOIP ponto a ponto com mídia hospedada pelo aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb6a5-141">Create peer to peer VOIP call with application hosted media</span></span>

> <span data-ttu-id="fb6a5-142">Observação: precisa de calls. initiate. All e calls. AccessMedia. All.</span><span class="sxs-lookup"><span data-stu-id="fb6a5-142">Note: Needs Calls.Initiate.All and Calls.AccessMedia.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="fb6a5-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb6a5-143">Request</span></span>
<span data-ttu-id="fb6a5-144">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb6a5-144">The following example shows the request.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  },
  "requestedModalities": [ "audio" ],
  "source": {
    "identity": {
      "application": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "IT Bot"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "subject": "Test Call",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      }
    }
  ],
  "tenantId": "tenantId-value"
}
```

### <a name="create-group-call-with-service-hosted-media"></a><span data-ttu-id="fb6a5-145">Criar uma chamada de grupo com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="fb6a5-145">Create group call with service hosted media</span></span>

> <span data-ttu-id="fb6a5-146">**Observação:** Este exemplo precisa das permissões calls. InitiateGroupCalls. All e calls. AccessMedia. All.</span><span class="sxs-lookup"><span data-stu-id="fb6a5-146">**Note:** This example needs the Calls.InitiateGroupCalls.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="fb6a5-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb6a5-147">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "targets": [
    {
      "identity": {
        "user": {
          "id": "29362BD4-CD58-4ED0-A206-0E4A33DBB0B6",
          "displayName": "Heidi Steen"
        }
      }
    },
    {
      "identity": {
        "phone": {
          "displayName": "+12345678890",
          "id": "+12345678890"
        }
      }
    }
  ],
  "requestedModalities": [ "audio", "video" ],
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
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "0",
    "replyChainMessageId": null
  }
}
```

### <a name="join-private-meeting-with-service-hosted-media"></a><span data-ttu-id="fb6a5-148">Ingressar em reunião privada com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="fb6a5-148">Join private meeting with service hosted media</span></span>

> <span data-ttu-id="fb6a5-149">**Observação:** Este exemplo precisa da permissão calls. JoinGroupCalls. All.</span><span class="sxs-lookup"><span data-stu-id="fb6a5-149">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="fb6a5-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb6a5-150">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "requestedModalities": [ "audio", "video" ],
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
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
        "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
      }
    }
  }
}
```

### <a name="join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="fb6a5-151">Reunião de canal de ingresso com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="fb6a5-151">Join channel meeting with service hosted media</span></span>

> <span data-ttu-id="fb6a5-152">**Observação:** Este exemplo precisa da permissão calls. JoinGroupCalls. All.</span><span class="sxs-lookup"><span data-stu-id="fb6a5-152">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="fb6a5-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb6a5-153">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "requestedModalities": [ "audio", "video" ],
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
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "1507228578052",
    "replyChainMessageId": null
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
        "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
      }
    }
  }
}
```

### <a name="join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="fb6a5-154">Ingressar na reunião de canal como um convidado com mídia de serviço hospedado</span><span class="sxs-lookup"><span data-stu-id="fb6a5-154">Join channel meeting as a guest with service hosted media</span></span>

> <span data-ttu-id="fb6a5-155">**Observação:** Este exemplo precisa da permissão calls. JoinGroupCallsAsGuest. All.</span><span class="sxs-lookup"><span data-stu-id="fb6a5-155">**Note:** This example needs the Calls.JoinGroupCallsAsGuest.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="fb6a5-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb6a5-156">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```
<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "user": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698",
        "displayName": "App_Guest_DisplayName",
        "identityProvider": "None"
      }
    }
  },
  "requestedModalities": [ "audio", "video" ],
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
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "1507228578052",
    "replyChainMessageId": null
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
        "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
      }
    }
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
    "Error: /api-reference/beta/api/application-post-calls.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
