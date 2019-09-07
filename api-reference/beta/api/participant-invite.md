---
title: 'participante: convidar'
description: Convide participantes para a chamada ativa.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aa463a7b300cfc4f3e6a8ad27bf2a7344b41c09d
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792517"
---
# <a name="participant-invite"></a><span data-ttu-id="236c7-103">participante: convidar</span><span class="sxs-lookup"><span data-stu-id="236c7-103">participant: invite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="236c7-104">Convide os participantes para a chamada de multipartes ativa.</span><span class="sxs-lookup"><span data-stu-id="236c7-104">Invite participants to the active multiparty call.</span></span>

<span data-ttu-id="236c7-105">Para obter mais informações sobre como lidar com operações de convite de participante de longa duração, consulte [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md).</span><span class="sxs-lookup"><span data-stu-id="236c7-105">For more information about how to handle long-running participant invitation operations, see [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md).</span></span>

><span data-ttu-id="236c7-106">**Observação:** Essa API tem suporte apenas para chamadas de vários participantes.</span><span class="sxs-lookup"><span data-stu-id="236c7-106">**Note:** This API is only supported for multiparty calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="236c7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="236c7-107">Permissions</span></span>
<span data-ttu-id="236c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="236c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="236c7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="236c7-110">Permission type</span></span> | <span data-ttu-id="236c7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="236c7-111">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="236c7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="236c7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="236c7-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="236c7-113">Not Supported</span></span>                       |
| <span data-ttu-id="236c7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="236c7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="236c7-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="236c7-115">Not Supported</span></span>                       |
| <span data-ttu-id="236c7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="236c7-116">Application</span></span>     | <span data-ttu-id="236c7-117">Calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="236c7-117">Calls.InitiateGroupCalls.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="236c7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="236c7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/invite
```

## <a name="request-headers"></a><span data-ttu-id="236c7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="236c7-119">Request headers</span></span>
| <span data-ttu-id="236c7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="236c7-120">Name</span></span>          | <span data-ttu-id="236c7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="236c7-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="236c7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="236c7-122">Authorization</span></span> | <span data-ttu-id="236c7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="236c7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="236c7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="236c7-125">Request body</span></span>
<span data-ttu-id="236c7-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="236c7-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="236c7-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="236c7-127">Parameter</span></span>      | <span data-ttu-id="236c7-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="236c7-128">Type</span></span>    |<span data-ttu-id="236c7-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="236c7-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="236c7-130">participants</span><span class="sxs-lookup"><span data-stu-id="236c7-130">participants</span></span>|<span data-ttu-id="236c7-131">coleção [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="236c7-131">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>| <span data-ttu-id="236c7-132">Os participantes a serem convidados.</span><span class="sxs-lookup"><span data-stu-id="236c7-132">The participants to invite.</span></span>|
|<span data-ttu-id="236c7-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="236c7-133">clientContext</span></span>|<span data-ttu-id="236c7-134">String</span><span class="sxs-lookup"><span data-stu-id="236c7-134">String</span></span>|<span data-ttu-id="236c7-135">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="236c7-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="236c7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="236c7-136">Response</span></span>
<span data-ttu-id="236c7-137">Se tiver êxito, esta API retornará `202 Accepted` um código de resposta e um cabeçalho de local com um URI para o objeto [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="236c7-137">If successful, this API returns a `202 Accepted` response code and a Location header with a URI to the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) object created for this request.</span></span> <span data-ttu-id="236c7-138">O corpo da resposta contém o [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) criado.</span><span class="sxs-lookup"><span data-stu-id="236c7-138">The body of the response contains the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) created.</span></span>

## <a name="examples"></a><span data-ttu-id="236c7-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="236c7-139">Examples</span></span>
<span data-ttu-id="236c7-140">Os exemplos a seguir mostram como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="236c7-140">The following examples shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="236c7-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="236c7-141">Request</span></span>
<span data-ttu-id="236c7-142">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="236c7-142">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="236c7-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="236c7-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="236c7-144">C#</span><span class="sxs-lookup"><span data-stu-id="236c7-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="236c7-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="236c7-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="236c7-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="236c7-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="236c7-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="236c7-147">Response</span></span>

> <span data-ttu-id="236c7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="236c7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
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
<br/>

## <a name="example---invite-participants-to-an-existing-multiparty-call"></a><span data-ttu-id="236c7-150">Exemplo: Convide os participantes para uma chamada de multiparts existente</span><span class="sxs-lookup"><span data-stu-id="236c7-150">Example - Invite participants to an existing multiparty call</span></span>

##### <a name="request"></a><span data-ttu-id="236c7-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="236c7-151">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="236c7-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="236c7-152">Response</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="236c7-153">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="236c7-153">Notification - operation completed</span></span>

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
  "@odata.type": "microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"51\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="236c7-154">Notificação-lista atualizada com o participante adicionado</span><span class="sxs-lookup"><span data-stu-id="236c7-154">Notification - roster updated with participant added</span></span>

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
  "@odata.type": "microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "microsoft.graph.commsNotification",
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

## <a name="example---invite-participants-to-a-multiparty-call-replacing-an-existing-peer-to-peer-call"></a><span data-ttu-id="236c7-155">Exemplo: Convide os participantes para uma chamada de várias partes, substituindo uma chamada ponto a ponto existente</span><span class="sxs-lookup"><span data-stu-id="236c7-155">Example - Invite participants to a multiparty call, replacing an existing peer-to-peer call</span></span>

<span data-ttu-id="236c7-156">Este exemplo pressupõe que uma chamada ponto a ponto existente tenha sido estabelecida entre o bot e o usuário com ID `8A34A46B-3D17-4ADC-8DCE-DC4E7D572698`, e gostaríamos de convidar o usuário para uma chamada de vários participantes existente enquanto encerrasse a chamada ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="236c7-156">This example assumes an existing peer-to-peer call has been established between the bot and user with ID `8A34A46B-3D17-4ADC-8DCE-DC4E7D572698`, and we'd like the bot to invite the user into an existing multiparty call while ending the peer-to-peer call.</span></span>

<span data-ttu-id="236c7-157">Para obter detalhes sobre `replacesCallId` como usar o para substituir uma chamada ponto a ponto existente, confira [participante do convite](../resources/invitationparticipantinfo.md).</span><span class="sxs-lookup"><span data-stu-id="236c7-157">For details on using `replacesCallId` to replace an existing peer-to-peer call, see [Invitation Participant](../resources/invitationparticipantinfo.md).</span></span>

##### <a name="request"></a><span data-ttu-id="236c7-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="236c7-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="236c7-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="236c7-159">Response</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="236c7-160">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="236c7-160">Notification - Operation completed</span></span>

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
  "@odata.type": "microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "microsoft.graph.commsNotification",
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

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="236c7-161">Notificação-lista atualizada com o participante adicionado</span><span class="sxs-lookup"><span data-stu-id="236c7-161">Notification - Roster updated with participant added</span></span>

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
  "@odata.type": "microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "microsoft.graph.commsNotification",
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

##### <a name="notification---terminated-the-original-peer-to-peer-call"></a><span data-ttu-id="236c7-162">Notificação – encerrada a chamada ponto a ponto original</span><span class="sxs-lookup"><span data-stu-id="236c7-162">Notification - Terminated the original peer-to-peer call</span></span>

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
  "@odata.type": "microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "microsoft.graph.commsNotification",
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

##### <a name="notification---deleted-the-original-peer-to-peer-call"></a><span data-ttu-id="236c7-163">Notification-exclusão da chamada ponto a ponto original</span><span class="sxs-lookup"><span data-stu-id="236c7-163">Notification - Deleted the original peer-to-peer call</span></span>

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
  "@odata.type": "microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "microsoft.graph.commsNotification",
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

## <a name="example---invite-participant-failure"></a><span data-ttu-id="236c7-164">Exemplo-convidar falha do participante</span><span class="sxs-lookup"><span data-stu-id="236c7-164">Example - Invite Participant Failure</span></span>

<span data-ttu-id="236c7-165">No caso de falha da operação de convite do participante, o bot receberá uma notificação [](../resources/inviteparticipantsoperation.md) com o `status` inviteParticipantsOperation com `failed`definido como.</span><span class="sxs-lookup"><span data-stu-id="236c7-165">In the event the invite participant operation fails, the bot will receive a notification with the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) with `status` set to `failed`.</span></span>

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
  "@odata.type": "microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resource": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
        "@odata.id": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"51\"",
        "clientContext": "A904FBD5A31041E881E861877A3DE3CD",
        "status": "failed",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 500,
          "subCode": 0,
          "message": "addParticipantsfailed for participants: 28:8A34A46B-3D17-4ADC-8DCE-DC4E7D572698 reason: Audio-video modality controller could not invite participant to this conversation., code=580 subcode=5201"
        },
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
  ]
}
-->
