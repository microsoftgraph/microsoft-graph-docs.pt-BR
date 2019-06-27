---
title: 'participante: convidar'
description: Convide participantes para a chamada ativa.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 06a89b42c437659aa2d4f1b521e6bacb795333f2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268492"
---
# <a name="participant-invite"></a><span data-ttu-id="02732-103">participante: convidar</span><span class="sxs-lookup"><span data-stu-id="02732-103">participant: invite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02732-104">Convide participantes para a chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="02732-104">Invite participants to the active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="02732-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="02732-105">Permissions</span></span>
<span data-ttu-id="02732-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02732-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02732-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02732-108">Permission type</span></span> | <span data-ttu-id="02732-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02732-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="02732-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02732-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="02732-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="02732-111">Not Supported</span></span>                       |
| <span data-ttu-id="02732-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02732-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02732-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="02732-113">Not Supported</span></span>                       |
| <span data-ttu-id="02732-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02732-114">Application</span></span>     | <span data-ttu-id="02732-115">Calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="02732-115">Calls.InitiateGroupCalls.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="02732-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02732-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/invite
POST /applications/{id}/calls/{id}/participants/invite
```

## <a name="request-headers"></a><span data-ttu-id="02732-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02732-117">Request headers</span></span>
| <span data-ttu-id="02732-118">Nome</span><span class="sxs-lookup"><span data-stu-id="02732-118">Name</span></span>          | <span data-ttu-id="02732-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="02732-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="02732-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="02732-120">Authorization</span></span> | <span data-ttu-id="02732-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02732-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02732-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02732-123">Request body</span></span>
<span data-ttu-id="02732-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02732-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="02732-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="02732-125">Parameter</span></span>      | <span data-ttu-id="02732-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="02732-126">Type</span></span>    |<span data-ttu-id="02732-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="02732-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02732-128">participants</span><span class="sxs-lookup"><span data-stu-id="02732-128">participants</span></span>|<span data-ttu-id="02732-129">coleção [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="02732-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>| <span data-ttu-id="02732-130">Os participantes a serem convidados.</span><span class="sxs-lookup"><span data-stu-id="02732-130">The participants to invite.</span></span>|
|<span data-ttu-id="02732-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="02732-131">clientContext</span></span>|<span data-ttu-id="02732-132">String</span><span class="sxs-lookup"><span data-stu-id="02732-132">String</span></span>|<span data-ttu-id="02732-133">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="02732-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="02732-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="02732-134">Response</span></span>
<span data-ttu-id="02732-135">Retorna `202 Accepted` o código de resposta e um cabeçalho de local com um URI para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="02732-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="examples"></a><span data-ttu-id="02732-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="02732-136">Examples</span></span>
<span data-ttu-id="02732-137">Os exemplos a seguir mostram como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="02732-137">The following examples shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="02732-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02732-138">Request</span></span>
<span data-ttu-id="02732-139">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="02732-139">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "participant-invite"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/invite
Content-Type: application/json
Content-Length: 464

{
  "participants": [
    {
      "endpointType": "default",
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "languageId-value",
      "region": "region-value",
      "replacesCallId": "replacesCallId-value"
    }
  ],
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="02732-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="02732-140">Response</span></span>

> <span data-ttu-id="02732-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02732-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="02732-143">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="02732-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="02732-144">C#</span><span class="sxs-lookup"><span data-stu-id="02732-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/participant-invite-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02732-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="02732-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/participant-invite-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="02732-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="02732-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/participant-invite-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<br/>

### <a name="invite-participants-in-existing-p2p-meeting"></a><span data-ttu-id="02732-147">Convidar participantes na reunião P2P existente</span><span class="sxs-lookup"><span data-stu-id="02732-147">Invite Participants in Existing P2P meeting</span></span>

##### <a name="request"></a><span data-ttu-id="02732-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02732-148">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/invite
Content-Type: application/json

{
  "participants": [
    {
      "endpointType": "default",
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "en-US",
      "region": "westus"
    }
  ],
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="02732-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="02732-149">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "running",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="02732-150">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="02732-150">Notification - operation completed</span></span>

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
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"51\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="02732-151">Notificação-lista atualizada com o participante adicionado</span><span class="sxs-lookup"><span data-stu-id="02732-151">Notification - roster updated with participant added</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/8A34A46B3D174ADC8DCEDC4E7D572698",
          "@odata.etag": "W/\"51\"",
          "info": {
            "identity": {
              "user": {
                "displayName": "Test User",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ]
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/123456W77E24E4D85F80597083CB830",
          "@odata.etag": "W/\"55\"",
          "info": {
            "identity": {
              "application": {
                "displayName": "Test Bot",
                "id": "1234A46B-3D17-4ADC-8DCE-DC4E7D556789"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ]
        }
      ]
    }
  ]
}
```

### <a name="invite-participants-in-existing-p2p-meeting"></a><span data-ttu-id="02732-152">Convidar participantes na reunião P2P existente</span><span class="sxs-lookup"><span data-stu-id="02732-152">Invite Participants in Existing P2P meeting</span></span>

<span data-ttu-id="02732-153">Este exemplo mostra um fluxo de E2E completo para [convidar participantes](../api/participant-invite.md) em uma reunião P2P existente.</span><span class="sxs-lookup"><span data-stu-id="02732-153">This example shows a complete E2E flow for [Invite Participants](../api/participant-invite.md) in an existing P2P meeting.</span></span>

##### <a name="answer-incoming-voip-call-with-service-hosted-media"></a><span data-ttu-id="02732-154">Atender a chamada VOIP de entrada com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="02732-154">Answer Incoming VOIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="02732-155">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="02732-155">Notification - Incoming</span></span>

``` http
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
      "changeType": "created",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "user": {
              "displayName": "Test User",
              "language": "en-US",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          }
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "language": "en-US",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            }
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="02732-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02732-156">Request</span></span>

``` http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "callback": "https://bot.contoso.com/api/calls",
  "acceptModalities": [ "audio", "video" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
      {
        "url": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        "url": "https://cdn.contoso.com/cool.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="02732-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="02732-157">Response</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 306

{
  "clientContext": "clientContext-value",
  "createdDateTime": "2018-03-19T09:46:02Z",
  "id": "id-value",
  "lastActionDateTime": "2018-03-19T09:46:02Z",
  "status": "Running"
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="02732-158">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="02732-158">Notification - Establishing</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="02732-159">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="02732-159">Notification - Established</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established",
        "activeModalities": [ "audio", "video" ],
        "requestedModalities": []
      }
    }
  ]
}
```

### <a name="join-channel-meeting-without-media"></a><span data-ttu-id="02732-160">Reunião de canal de ingresso sem mídia</span><span class="sxs-lookup"><span data-stu-id="02732-160">Join channel meeting without media</span></span>

> <span data-ttu-id="02732-161">**Importante**: se a instância de bot estiver ingressando somente no objetivo de facilitar a transferência, ela deve evitar negociações de mídia.</span><span class="sxs-lookup"><span data-stu-id="02732-161">**IMPORTANT**: If the bot instance is joining only for the purpose of facilitating the transfer, it should avoid media negotiations.</span></span>  <span data-ttu-id="02732-162">Portanto, é melhor adicioná-lo sem qualquer um `requestedModalities` ou `mediaConfig`.</span><span class="sxs-lookup"><span data-stu-id="02732-162">Therefore, it is best to add it without any `requestedModalities` or `mediaConfig`.</span></span>

##### <a name="request"></a><span data-ttu-id="02732-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02732-163">Request</span></span>

``` http
POST /app/calls
Content-Type: application/json

{
  "subject": "Test Call",
  "callback": "https://bot.contoso.com/api/calls",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "targetDisposition": "default",
  "requestedModalities": [],
  "chatInfo": {
    "threadId": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
    "messageId": "1507228578052",
    "replyChainMessageId": "1507228578052"
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

##### <a name="response"></a><span data-ttu-id="02732-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="02732-164">Response</span></span>

``` http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/app/calls/90ED37DCD8E34E119DE330A955DDA06F
```

##### <a name="notification---establishing"></a><span data-ttu-id="02732-165">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="02732-165">Notification - Establishing</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing",
        "direction": "outgoing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="02732-166">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="02732-166">Notification - Established</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F",
        "@odata.etag": "W/\"5445\"",
        "state": "established",
        "activeModalities": []
      }
    }
  ]
}
```

### <a name="invite-participant-from-initial-incoming-call"></a><span data-ttu-id="02732-167">Convidar o participante da chamada de entrada inicial</span><span class="sxs-lookup"><span data-stu-id="02732-167">Invite participant from initial incoming call</span></span>

``` http
POST /app/calls/90ED37DCD8E34E119DE330A955DDA06F/participants/invite
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "user": {
          "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
        }
      },
      "replacesCallId": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896"
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="02732-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="02732-168">Response</span></span>

``` http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/90ED37DCD8E34E119DE330A955DDA06F/operations/0FE0623FD62842EDB4BD8AC290072CC5
Content-Type: application/json
Content-Length: 306

{
  "clientContext": "clientContext-value",
  "createdDateTime": "2018-03-19T09:46:02Z",
  "id": "id-value",
  "lastActionDateTime": "2018-03-19T09:46:02Z",
  "status": "Running"
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="02732-169">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="02732-169">Notification - Operation Completed</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
        "@odata.id": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"51\"",
        "clientContext": "A904FBD5A31041E881E861877A3DE3CD",
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="02732-170">Notificação-lista atualizada com o participante adicionado</span><span class="sxs-lookup"><span data-stu-id="02732-170">Notification - Roster Updated With Participant Added</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/8A34A46B3D174ADC8DCEDC4E7D572698",
          "@odata.etag": "W/\"51\"",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "user": {
                "region": "westus",
                "languageId": "en-US",
                "displayName": "Test User",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            }
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1",
              "direction": "sendReceive"
            }
          ]
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/123456W77E24E4D85F80597083CB830",
          "@odata.etag": "W/\"55\"",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "application": {
                "region": "westus",
                "languageId": "en-US",
                "displayName": "Test Bot",
                "id": "1234A46B-3D17-4ADC-8DCE-DC4E7D556789"
              }
            }
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2",
              "direction": "sendReceive"
            }
          ]
        }
      ]
    }
  ]
}
```

##### <a name="notification---terminated-the-original-p2p-call"></a><span data-ttu-id="02732-171">Notificação – finalizou a chamada P2P original</span><span class="sxs-lookup"><span data-stu-id="02732-171">Notification - terminated the original P2P call</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppInitiated"
      }
    }
  ]
}
```

##### <a name="notification---deleted-the-original-p2p-call"></a><span data-ttu-id="02732-172">Notification-exclusão da chamada P2P original</span><span class="sxs-lookup"><span data-stu-id="02732-172">Notification - Deleted the original P2P call</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\""
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
  "description": "participant: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/participant-invite.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/participant-invite.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/participant-invite.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
