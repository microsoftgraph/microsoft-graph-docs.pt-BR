---
title: Criar chamada
description: Crie uma nova chamada.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 1a2c6e85579e82787abf0bb7bb8b541c81aaf12e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818736"
---
# <a name="create-call"></a><span data-ttu-id="66e19-103">Criar chamada</span><span class="sxs-lookup"><span data-stu-id="66e19-103">Create call</span></span>

> <span data-ttu-id="66e19-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="66e19-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66e19-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="66e19-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66e19-106">Crie uma nova chamada.</span><span class="sxs-lookup"><span data-stu-id="66e19-106">Create a new call.</span></span>

## <a name="permissions"></a><span data-ttu-id="66e19-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="66e19-107">Permissions</span></span>
<span data-ttu-id="66e19-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66e19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66e19-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66e19-110">Permission type</span></span>                        | <span data-ttu-id="66e19-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66e19-111">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="66e19-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66e19-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="66e19-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="66e19-113">Not Supported</span></span>                                                                           |
| <span data-ttu-id="66e19-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66e19-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66e19-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="66e19-115">Not Supported</span></span>                                                                           |
| <span data-ttu-id="66e19-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66e19-116">Application</span></span>                            | <span data-ttu-id="66e19-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="66e19-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="66e19-118">**Observação:** Para uma chamada com a mídia do aplicativo hospedado, você precisa ter a permissão de Calls.AccessMedia.All com uma das permissões listadas na tabela anterior.</span><span class="sxs-lookup"><span data-stu-id="66e19-118">**Note:** For a call with app hosted media, you need the Calls.AccessMedia.All permission with one of the permissions listed in the previous table.</span></span>

## <a name="http-request"></a><span data-ttu-id="66e19-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66e19-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
POST /applications/{id}/calls
```

## <a name="request-headers"></a><span data-ttu-id="66e19-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66e19-120">Request headers</span></span>
| <span data-ttu-id="66e19-121">Nome</span><span class="sxs-lookup"><span data-stu-id="66e19-121">Name</span></span>          | <span data-ttu-id="66e19-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="66e19-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="66e19-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="66e19-123">Authorization</span></span> | <span data-ttu-id="66e19-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66e19-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66e19-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66e19-126">Request body</span></span>
<span data-ttu-id="66e19-127">No corpo da solicitação, fornece uma representação JSON de um objeto de [chamada](../resources/call.md) .</span><span class="sxs-lookup"><span data-stu-id="66e19-127">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

> <span data-ttu-id="66e19-128">**Observação:** Propriedades marcadas como `Server generated` serão ignorados durante o processamento `POST` em `app/calls`.</span><span class="sxs-lookup"><span data-stu-id="66e19-128">**Note:** Properties marked as `Server generated` are ignored when processing `POST` on `app/calls`.</span></span>

## <a name="response"></a><span data-ttu-id="66e19-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="66e19-129">Response</span></span>
<span data-ttu-id="66e19-130">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto de [chamada](../resources/call.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66e19-130">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66e19-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="66e19-131">Examples</span></span>

### <a name="create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="66e19-132">Criar chamada VOIP de ponto a ponto com mídia de serviço hospedado</span><span class="sxs-lookup"><span data-stu-id="66e19-132">Create peer to peer VOIP call with service hosted media</span></span>

> <span data-ttu-id="66e19-133">**Observação:** Essa chamada precisa a permissão Calls.Initiate.All.</span><span class="sxs-lookup"><span data-stu-id="66e19-133">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="66e19-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66e19-134">Request</span></span>
<span data-ttu-id="66e19-135">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="66e19-135">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="66e19-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="66e19-136">Response</span></span>

> <span data-ttu-id="66e19-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66e19-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---establishing"></a><span data-ttu-id="66e19-139">Notificação - estabelecendo</span><span class="sxs-lookup"><span data-stu-id="66e19-139">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="66e19-140">Notificação - estabelecida</span><span class="sxs-lookup"><span data-stu-id="66e19-140">Notification - established</span></span>

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

### <a name="create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="66e19-141">Criar chamada VOIP de ponto a ponto com mídia de aplicativo hospedado</span><span class="sxs-lookup"><span data-stu-id="66e19-141">Create peer to peer VOIP call with application hosted media</span></span>

> <span data-ttu-id="66e19-142">Observação: Precisa permissão Calls.Initiate.All e Calls.AccessMedia.All.</span><span class="sxs-lookup"><span data-stu-id="66e19-142">Note: Needs Calls.Initiate.All and Calls.AccessMedia.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="66e19-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66e19-143">Request</span></span>
<span data-ttu-id="66e19-144">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="66e19-144">The following example shows the request.</span></span>

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

### <a name="create-group-call-with-service-hosted-media"></a><span data-ttu-id="66e19-145">Criar grupo de chamada com mídia de serviço hospedado</span><span class="sxs-lookup"><span data-stu-id="66e19-145">Create group call with service hosted media</span></span>

> <span data-ttu-id="66e19-146">**Observação:** Este exemplo precisa as permissões Calls.InitiateGroupCalls.All e Calls.AccessMedia.All.</span><span class="sxs-lookup"><span data-stu-id="66e19-146">**Note:** This example needs the Calls.InitiateGroupCalls.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="66e19-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66e19-147">Request</span></span>

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

### <a name="join-private-meeting-with-service-hosted-media"></a><span data-ttu-id="66e19-148">Ingressar na reunião privada com mídia de serviço hospedado</span><span class="sxs-lookup"><span data-stu-id="66e19-148">Join private meeting with service hosted media</span></span>

> <span data-ttu-id="66e19-149">**Observação:** Este exemplo precisa a permissão Calls.JoinGroupCalls.All.</span><span class="sxs-lookup"><span data-stu-id="66e19-149">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="66e19-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66e19-150">Request</span></span>

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

### <a name="join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="66e19-151">Ingressar em reunião de canal com mídia de serviço hospedado</span><span class="sxs-lookup"><span data-stu-id="66e19-151">Join channel meeting with service hosted media</span></span>

> <span data-ttu-id="66e19-152">**Observação:** Este exemplo precisa a permissão Calls.JoinGroupCalls.All.</span><span class="sxs-lookup"><span data-stu-id="66e19-152">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="66e19-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66e19-153">Request</span></span>

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

### <a name="join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="66e19-154">Ingressar em reunião de canal como convidado com mídia de serviço hospedado</span><span class="sxs-lookup"><span data-stu-id="66e19-154">Join channel meeting as a guest with service hosted media</span></span>

> <span data-ttu-id="66e19-155">**Observação:** Este exemplo precisa a permissão Calls.JoinGroupCallsAsGuest.All.</span><span class="sxs-lookup"><span data-stu-id="66e19-155">**Note:** This example needs the Calls.JoinGroupCallsAsGuest.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="66e19-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66e19-156">Request</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create call",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
