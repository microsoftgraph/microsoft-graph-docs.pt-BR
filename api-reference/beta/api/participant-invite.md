---
title: 'participante: invite'
description: Convide participantes para a chamada ativa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ac0436723a8e01d3476990f3d794b8fcd0e7ed9f
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666356"
---
# <a name="participant-invite"></a><span data-ttu-id="4d031-103">participante: invite</span><span class="sxs-lookup"><span data-stu-id="4d031-103">participant: invite</span></span>

<span data-ttu-id="4d031-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d031-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d031-105">Convide participantes para a chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="4d031-105">Invite participants to the active call.</span></span>

<span data-ttu-id="4d031-106">Para obter mais informações sobre como lidar com operações, consulte [commsoperation](../resources/commsoperation.md).</span><span class="sxs-lookup"><span data-stu-id="4d031-106">For more information about how to handle operations, see [commsoperation](../resources/commsoperation.md).</span></span>

><span data-ttu-id="4d031-107">**Observação:** Essa API só tem suporte para chamadas de grupo.</span><span class="sxs-lookup"><span data-stu-id="4d031-107">**Note:** This API is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d031-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d031-108">Permissions</span></span>
<span data-ttu-id="4d031-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d031-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d031-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d031-111">Permission type</span></span> | <span data-ttu-id="4d031-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d031-112">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="4d031-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d031-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d031-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4d031-114">Not supported</span></span>                       |
| <span data-ttu-id="4d031-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d031-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d031-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4d031-116">Not supported</span></span>                       |
| <span data-ttu-id="4d031-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d031-117">Application</span></span>     | <span data-ttu-id="4d031-118">Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="4d031-118">Calls.InitiateGroupCalls.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="4d031-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d031-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/invite
POST /communications/calls/{id}/participants/invite
```
> <span data-ttu-id="4d031-120">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="4d031-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="4d031-121">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="4d031-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d031-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d031-122">Request headers</span></span>
| <span data-ttu-id="4d031-123">Nome</span><span class="sxs-lookup"><span data-stu-id="4d031-123">Name</span></span>          | <span data-ttu-id="4d031-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d031-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4d031-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d031-125">Authorization</span></span> | <span data-ttu-id="4d031-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d031-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d031-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="4d031-128">Content-type</span></span>  | <span data-ttu-id="4d031-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d031-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d031-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d031-131">Request body</span></span>
<span data-ttu-id="4d031-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d031-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4d031-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4d031-133">Parameter</span></span>      | <span data-ttu-id="4d031-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d031-134">Type</span></span>    |<span data-ttu-id="4d031-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d031-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d031-136">participants</span><span class="sxs-lookup"><span data-stu-id="4d031-136">participants</span></span>|<span data-ttu-id="4d031-137">conjunto [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="4d031-137">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>| <span data-ttu-id="4d031-138">Os participantes a serem convidados.</span><span class="sxs-lookup"><span data-stu-id="4d031-138">The participants to be invited.</span></span>|
|<span data-ttu-id="4d031-139">clientContext</span><span class="sxs-lookup"><span data-stu-id="4d031-139">clientContext</span></span>|<span data-ttu-id="4d031-140">String</span><span class="sxs-lookup"><span data-stu-id="4d031-140">String</span></span>|<span data-ttu-id="4d031-141">Cadeia de caracteres de contexto de cliente exclusiva.</span><span class="sxs-lookup"><span data-stu-id="4d031-141">Unique Client Context string.</span></span> <span data-ttu-id="4d031-142">O limite máximo é 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="4d031-142">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="4d031-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d031-143">Response</span></span>
<span data-ttu-id="4d031-144">Se succsessful, este método retorna um código de resposta e um header location com um URI para `200 OK` [o inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d031-144">If succsessful, this method returns a `200 OK` response code and a Location header with a URI to the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) created for this request.</span></span> <span data-ttu-id="4d031-145">O corpo da resposta contém [o inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) criado.</span><span class="sxs-lookup"><span data-stu-id="4d031-145">The body of the response contains the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) created.</span></span>

><span data-ttu-id="4d031-146">**Observação:** Quando essa API retornar uma resposta bem-sucedida, todos os participantes receberão uma atualização de lista.</span><span class="sxs-lookup"><span data-stu-id="4d031-146">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>


## <a name="examples"></a><span data-ttu-id="4d031-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4d031-147">Examples</span></span>
<span data-ttu-id="4d031-148">Os exemplos a seguir mostram como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="4d031-148">The following examples show how to call this API.</span></span>

> <span data-ttu-id="4d031-149">**Observação:** Os objetos de resposta podem ser reduzidos para a capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="4d031-149">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="4d031-150">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d031-150">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-invite-one-participant-to-an-existing-group-call"></a><span data-ttu-id="4d031-151">Exemplo 1: convidar um participante para uma chamada de grupo existente</span><span class="sxs-lookup"><span data-stu-id="4d031-151">Example 1: Invite one participant to an existing group call</span></span>

#### <a name="request"></a><span data-ttu-id="4d031-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d031-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4d031-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d031-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite-1"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/participants/invite
Content-Type: application/json
Content-Length: 464

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "278405a3-f568-4b3e-b684-009193463064",
          "identityProvider": "AAD"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="4d031-154">C#</span><span class="sxs-lookup"><span data-stu-id="4d031-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d031-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d031-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d031-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d031-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4d031-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d031-157">Response</span></span>

> <span data-ttu-id="4d031-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4d031-158">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
  "id": "eec3812a-fdc3-4fb4-825c-a06c9f35414e",
  "status": "Running",
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
  "resultInfo": null,
  "participants": [
    {
      "endpointType": null,
      "id": null,
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "user": {
          "id": "278405a3-f568-4b3e-b684-009193463064",
          "identityProvider": "AAD",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47"
        },
        "application": null,
        "device": null,
        "phone": null
      }
    }
  ]
}
```

#### <a name="notification---operation-completed"></a><span data-ttu-id="4d031-159">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="4d031-159">Notification - operation completed</span></span>

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
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[ 
      { 
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"deleted",
         "resource":"/app/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/eec3812a-fdc3-4fb4-825c-a06c9f35414e",
         "resourceUrl":"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/eec3812a-fdc3-4fb4-825c-a06c9f35414e",
         "resourceData":{ 
            "@odata.type":"#microsoft.graph.inviteParticipantsOperation",
            "participants":[ 
               { 
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{ 
                     "@odata.type":"#microsoft.graph.identitySet",
                     "user":{ 
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"278405a3-f568-4b3e-b684-009193463064",
                        "identityProvider":"AAD",
                        "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
                     }
                  }
               }
            ],
            "status":"completed",
            "clientContext":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
            "id":"eec3812a-fdc3-4fb4-825c-a06c9f35414e"
         }
      }
   ]
}
```

#### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="4d031-160">Notificação - lista atualizada com participante adicionado</span><span class="sxs-lookup"><span data-stu-id="4d031-160">Notification - roster updated with participant added</span></span>

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
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[
      {
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"updated",
         "resource":"/app/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants",
         "resourceUrl":"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants",
         "resourceData":[
            {
               "@odata.type":"#microsoft.graph.participant",
               "info":{
                  "@odata.type":"#microsoft.graph.participantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "application":{
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"278405a3-f568-4b3e-b684-009193463064",
                        "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
                     }
                  },
                  "endpointType":"default"
               },
               "mediaStreams":[
                  {
                     "@odata.type":"#microsoft.graph.mediaStream",
                     "mediaType":"audio",
                     "sourceId":"1",
                     "direction":"sendReceive",
                     "serverMuted":false
                  }
               ],
               "isMuted":false,
               "isInLobby":false,
               "id":null
            }
         ]
      }
   ]
}

```

### <a name="example-2-invite-multiple-participants-to-an-existing-group-call"></a><span data-ttu-id="4d031-161">Exemplo 2: convidar vários participantes para uma chamada de grupo existente</span><span class="sxs-lookup"><span data-stu-id="4d031-161">Example 2: Invite multiple participants to an existing group call</span></span>

> <span data-ttu-id="4d031-162">**Observação**: a chamada de grupo existente deve ter um [chatInfo válido.](../resources/chatInfo.md)</span><span class="sxs-lookup"><span data-stu-id="4d031-162">**Note**: The existing group call must have a valid [chatInfo](../resources/chatInfo.md).</span></span> <span data-ttu-id="4d031-163">Há suporte para convidar até 5 participantes.</span><span class="sxs-lookup"><span data-stu-id="4d031-163">Inviting up to 5 participants is supported.</span></span>

#### <a name="request"></a><span data-ttu-id="4d031-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d031-164">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4d031-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d031-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite-multiple"
}-->

```http
POST /communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/invite
Content-Type: application/json

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          "identityProvider": "AAD"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "1e126418-44a0-4a94-a6f8-0efe1ad71acb",
          "identityProvider": "AAD"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="4d031-166">C#</span><span class="sxs-lookup"><span data-stu-id="4d031-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-multiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d031-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d031-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-multiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d031-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d031-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-multiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="4d031-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d031-169">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
   "id":"eec3812a-fdc3-4fb4-825c-a06c9f35414e",
   "status":"Running",
   "clientContext":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
   "resultInfo":null,
   "participants":[
      {
         "endpointType":null,
         "id":null,
         "replacesCallId":null,
         "identity":{
            "user":{
               "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
               "identityProvider":"AAD",
               "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
            },
            "application":null,
            "device":null,
            "phone":null
         }
      },
      {
         "endpointType":null,
         "id":null,
         "replacesCallId":null,
         "identity":{
            "user":{
               "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
               "identityProvider":"AAD",
               "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
            },
            "application":null,
            "device":null,
            "phone":null
         }
      }
   ]
}

```
#### <a name="notification---operation-completed"></a><span data-ttu-id="4d031-170">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="4d031-170">Notification - operation completed</span></span>
```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```
<!-- {
  "blockType": "example",
  "truncated": "true",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resource": "/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/operations/participants",
      "resourceUrl": "/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/operations/participants",
      "resourceData": {
        "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
        "participants": [
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                "identityProvider":"AAD",
                "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
              }
            }
          },
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
                "identityProvider":"AAD",
                "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
              }
            }
          }
        ],
        "status": "completed",
        "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
        "id": null
      }
    }
  ]
}

```
#### <a name="notification---roster-updated-with-participants-added"></a><span data-ttu-id="4d031-171">Notificação - lista atualizada com participantes adicionados</span><span class="sxs-lookup"><span data-stu-id="4d031-171">Notification - roster updated with participants added</span></span>
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
      "resource": "/app/calls/7531d31f-d10d-44de-802f-c569dbca451c/operations/participants",
      "resourceUrl": "/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/operations/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47"
              }
            },
            "endpointType": "default"
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
                "mediaType": "audio",
              "sourceId": "1",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "id": null
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
                "identityProvider":"AAD",
                "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
             }
            },
            "endpointType": "default"
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "sourceId": "3",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "id": null
        }
      ]
    }
  ]
}


```

### <a name="example-3-invite-participants-to-a-an-existing-group-call-replacing-an-existing-peer-to-peer-call"></a><span data-ttu-id="4d031-172">Exemplo 3: convidar participantes para uma chamada de grupo existente, substituindo uma chamada ponto a ponto existente</span><span class="sxs-lookup"><span data-stu-id="4d031-172">Example 3: Invite participants to a an existing group call, replacing an existing Peer-to-Peer call</span></span>


<span data-ttu-id="4d031-173">A API de convite dá suporte a apenas um participante ao substituir uma chamada ponto a ponto existente.</span><span class="sxs-lookup"><span data-stu-id="4d031-173">The invite API supports only one participant when replacing an existing peer-to-peer call.</span></span> <span data-ttu-id="4d031-174">Quando vários participantes são fornecidos no corpo da solicitação, apenas o primeiro participante será lido e o restante dos participantes será ignorado.</span><span class="sxs-lookup"><span data-stu-id="4d031-174">When multiple participants are provided in the request body, only the first participant will be read and the rest of the participants will be ignored.</span></span>


> <span data-ttu-id="4d031-175">**Observação:** A API de convite dá suporte a apenas um participante `replacesCallId` quando é fornecida.</span><span class="sxs-lookup"><span data-stu-id="4d031-175">**Note:** The invite API supports only one participant when `replacesCallId` is provided.</span></span> 
> <span data-ttu-id="4d031-176">Para obter detalhes sobre como usar para substituir uma chamada ponto a ponto `replacesCallId` existente, consulte [invitationParticipantInfo](../resources/invitationparticipantinfo.md).</span><span class="sxs-lookup"><span data-stu-id="4d031-176">For  details about using `replacesCallId` to replace an existing peer-to-peer call, see [invitationParticipantInfo](../resources/invitationparticipantinfo.md).</span></span>

#### <a name="request"></a><span data-ttu-id="4d031-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d031-177">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4d031-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d031-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite-existing"
}-->

```http
POST /communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants/invite
Content-Type: application/json

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          "identityProvider": "AAD"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="4d031-179">C#</span><span class="sxs-lookup"><span data-stu-id="4d031-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-existing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d031-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d031-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-existing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d031-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d031-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-existing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4d031-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d031-182">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": "true",
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
  "id": "278405a3-f568-4b3e-b684-009193463064",
  "status": "Running",
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
  "resultInfo": null,
  "participants": [
    {
      "endpointType": null,
      "id": null,
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "user": {
          "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          "displayName": "Participant",
          "identityProvider": "AAD",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47"
        },
        "application": null,
        "device": null,
        "phone": null
      }
    }
  ]
}
```

#### <a name="notification---operation-completed"></a><span data-ttu-id="4d031-183">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="4d031-183">Notification - operation completed</span></span>

``` http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->

```json
{ 
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[ 
      { 
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"deleted",
         "resource":"/app/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/278405a3-f568-4b3e-b684-009193463064",
         "resourceUrl":"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/278405a3-f568-4b3e-b684-009193463064",
         "resourceData":{ 
            "@odata.type":"#microsoft.graph.inviteParticipantsOperation",
            "participants":[ 
               { 
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{ 
                     "@odata.type":"#microsoft.graph.identitySet",
                     "user":{ 
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                        "identityProvider":"AAD",
                        "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
                     }
                  }
               }
            ],
            "status":"completed",
            "clientContext":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
            "id":"278405a3-f568-4b3e-b684-009193463064"
         }
      }
   ]
}
```

#### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="4d031-184">Notificação - lista atualizada com participante adicionado</span><span class="sxs-lookup"><span data-stu-id="4d031-184">Notification - roster updated with participant added</span></span>

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
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[
      {
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"updated",
         "resource":"/communications/calls/a7ebfb2d-871e-419c-87af-27290b22e8db/participants",
         "resourceUrl":"/communications/calls/a7ebfb2d-871e-419c-87af-27290b22e8db/participants",
         "resourceData":[
            {
               "@odata.type":"#microsoft.graph.participant",
               "info":{
                  "@odata.type":"#microsoft.graph.participantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "user":{ 
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                        "identityProvider":"AAD",
                        "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
                     }
                  },
                  "endpointType":"default"
               },
               "mediaStreams":[
                  {
                     "@odata.type":"#microsoft.graph.mediaStream",
                     "mediaType":"audio",
                     "sourceId":"1",
                     "direction":"sendReceive",
                     "serverMuted":false
                  }
               ],
               "isMuted":false,
               "isInLobby":false,
               "id":null
            }
         ]
      }
   ]
}
```

><span data-ttu-id="4d031-185">**Observação:** Com um status "concluído", você pode esperar receber notificações sobre como sua chamada ponto a ponto original foi encerrada e excluída.</span><span class="sxs-lookup"><span data-stu-id="4d031-185">**Note:** With a "completed" status, you can expect to receive notifications on how your original peer-to-peer call has been terminated and deleted.</span></span>

### <a name="example-4-invite-one-pstn-participant-to-an-existing-group-call"></a><span data-ttu-id="4d031-186">Exemplo 4: convidar um participante PSTN para uma chamada de grupo existente</span><span class="sxs-lookup"><span data-stu-id="4d031-186">Example 4: Invite one PSTN participant to an existing group call</span></span>

<span data-ttu-id="4d031-187">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="4d031-187">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="4d031-188">Para obter detalhes, [consulte Atribuir um número de telefone ao seu bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span><span class="sxs-lookup"><span data-stu-id="4d031-188">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>
> <span data-ttu-id="4d031-189">**Observação:** Telefone ID é o número de telefone no formato E.164.</span><span class="sxs-lookup"><span data-stu-id="4d031-189">**Note:** Phone ID is the phone number in E.164 format.</span></span>

#### <a name="request"></a><span data-ttu-id="4d031-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d031-190">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4d031-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d031-191">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite-2"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/participants/invite
Content-Type: application/json
Content-Length: 464

{
  "participants": [
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
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="4d031-192">C#</span><span class="sxs-lookup"><span data-stu-id="4d031-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d031-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d031-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4d031-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d031-194">Response</span></span>

> <span data-ttu-id="4d031-195">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4d031-195">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
  "id": "eec3812a-fdc3-4fb4-825c-a06c9f35414e",
  "status": "Running",
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
  "resultInfo": null,
  "participants": [
    {
      "endpointType": null,
      "id": null,
      "replacesCallId": null,
      "identity": {
        "user": null,
        "guest": null,
        "encrypted": null,
        "onPremises": null,
        "applicationInstance": null,
        "application": null,
        "device": null,
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      }
    }
  ]
}
```

#### <a name="notification---operation-completed"></a><span data-ttu-id="4d031-196">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="4d031-196">Notification - operation completed</span></span>

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
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[ 
      { 
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"deleted",
         "resource":"/app/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/eec3812a-fdc3-4fb4-825c-a06c9f35414e",
         "resourceUrl":"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/eec3812a-fdc3-4fb4-825c-a06c9f35414e",
         "resourceData":{ 
            "@odata.type":"#microsoft.graph.inviteParticipantsOperation",
            "participants":[ 
               { 
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{ 
                     "@odata.type":"#microsoft.graph.identitySet",
                     "phone": {
                        "@odata.type": "#microsoft.graph.identity",
                        "id": "+12345678901"
                     }
                  }
               }
            ],
            "status":"completed",
            "clientContext":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
            "id":"eec3812a-fdc3-4fb4-825c-a06c9f35414e"
         }
      }
   ]
}
```

#### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="4d031-197">Notificação - lista atualizada com participante adicionado</span><span class="sxs-lookup"><span data-stu-id="4d031-197">Notification - roster updated with participant added</span></span>

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
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[
      {
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"updated",
         "resource":"/app/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants",
         "resourceUrl":"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants",
         "resourceData":[
            {
               "@odata.type":"#microsoft.graph.participant",
               "info":{
                  "@odata.type":"#microsoft.graph.participantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "phone": {
                        "@odata.type": "#microsoft.graph.identity",
                        "id": "+12345678901"
                     }
                  },
                  "endpointType":"default"
               },
               "mediaStreams":[
                  {
                     "@odata.type":"#microsoft.graph.mediaStream",
                     "mediaType":"audio",
                     "sourceId":"1",
                     "direction":"sendReceive",
                     "serverMuted":false
                  }
               ],
               "isMuted":false,
               "isInLobby":false,
               "id":null
            }
         ]
      }
   ]
}

```

><span data-ttu-id="4d031-198">**Observação:** Com um status, você pode esperar receber notificações sobre como sua chamada ponto a ponto original foi `completed` encerrada e excluída.</span><span class="sxs-lookup"><span data-stu-id="4d031-198">**Note:** With a `completed` status, you can expect to receive notifications about how your original peer-to-peer call has been terminated and deleted.</span></span>

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


