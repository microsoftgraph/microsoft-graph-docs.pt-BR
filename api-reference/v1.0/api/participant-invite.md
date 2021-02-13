---
title: 'participante: invite'
description: Convide participantes para a chamada ativa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d4702e7257a5c49a8ef1232391dc923589bd2808
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177099"
---
# <a name="participant-invite"></a><span data-ttu-id="73911-103">participante: invite</span><span class="sxs-lookup"><span data-stu-id="73911-103">participant: invite</span></span>

<span data-ttu-id="73911-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73911-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73911-105">Convide participantes para a chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="73911-105">Invite participants to the active call.</span></span>

<span data-ttu-id="73911-106">Para obter mais informações sobre como lidar com operações, consulte [commsoperation](../resources/commsoperation.md).</span><span class="sxs-lookup"><span data-stu-id="73911-106">For more information about how to handle operations, see [commsoperation](../resources/commsoperation.md).</span></span>

><span data-ttu-id="73911-107">**Observação:** Essa API só é suportada para chamadas de grupo.</span><span class="sxs-lookup"><span data-stu-id="73911-107">**Note:** This API is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="73911-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="73911-108">Permissions</span></span>
<span data-ttu-id="73911-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73911-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73911-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73911-111">Permission type</span></span> | <span data-ttu-id="73911-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73911-112">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="73911-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73911-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="73911-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="73911-114">Not supported</span></span>                       |
| <span data-ttu-id="73911-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73911-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73911-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="73911-116">Not supported</span></span>                       |
| <span data-ttu-id="73911-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73911-117">Application</span></span>     | <span data-ttu-id="73911-118">Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="73911-118">Calls.InitiateGroupCalls.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="73911-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73911-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/participants/invite
```

## <a name="request-headers"></a><span data-ttu-id="73911-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73911-120">Request headers</span></span>
| <span data-ttu-id="73911-121">Nome</span><span class="sxs-lookup"><span data-stu-id="73911-121">Name</span></span>          | <span data-ttu-id="73911-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="73911-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="73911-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="73911-123">Authorization</span></span> | <span data-ttu-id="73911-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73911-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73911-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="73911-126">Content-type</span></span>  | <span data-ttu-id="73911-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73911-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73911-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73911-129">Request body</span></span>
<span data-ttu-id="73911-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73911-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="73911-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="73911-131">Parameter</span></span>      | <span data-ttu-id="73911-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="73911-132">Type</span></span>    |<span data-ttu-id="73911-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="73911-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73911-134">participants</span><span class="sxs-lookup"><span data-stu-id="73911-134">participants</span></span>|<span data-ttu-id="73911-135">conjunto [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="73911-135">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>| <span data-ttu-id="73911-136">Os participantes a serem convidados.</span><span class="sxs-lookup"><span data-stu-id="73911-136">The participants to be invited.</span></span>|
|<span data-ttu-id="73911-137">clientContext</span><span class="sxs-lookup"><span data-stu-id="73911-137">clientContext</span></span>|<span data-ttu-id="73911-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73911-138">String</span></span>|<span data-ttu-id="73911-139">Cadeia de caracteres de contexto de cliente exclusiva.</span><span class="sxs-lookup"><span data-stu-id="73911-139">Unique Client Context string.</span></span> <span data-ttu-id="73911-140">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="73911-140">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="73911-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="73911-141">Response</span></span>
<span data-ttu-id="73911-142">Se tiver sucesso, este método retornará um código de resposta e um header de local com um URI para `200 OK` [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="73911-142">If succsessful, this method returns a `200 OK` response code and a location header with a URI to the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) created for this request.</span></span> 

<span data-ttu-id="73911-143">O corpo da resposta contém o [inviteParticipantsOperation criado.](../resources/inviteparticipantsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="73911-143">The body of the response contains the created [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md).</span></span>

><span data-ttu-id="73911-144">**Observação:** Quando essa API retornar uma resposta bem-sucedida, todos os participantes receberão uma atualização da lista de participação.</span><span class="sxs-lookup"><span data-stu-id="73911-144">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>


## <a name="examples"></a><span data-ttu-id="73911-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="73911-145">Examples</span></span>
<span data-ttu-id="73911-146">Os exemplos a seguir mostram como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="73911-146">The following examples show how to call this API.</span></span>

> <span data-ttu-id="73911-147">**Observação:** Os objetos de resposta podem ser reduzidos para maior leitura.</span><span class="sxs-lookup"><span data-stu-id="73911-147">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="73911-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73911-148">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-invite-one-participant-to-an-existing-group-call"></a><span data-ttu-id="73911-149">Exemplo 1: Convidar um participante para uma chamada de grupo existente</span><span class="sxs-lookup"><span data-stu-id="73911-149">Example 1: Invite one participant to an existing group call</span></span>

##### <a name="request"></a><span data-ttu-id="73911-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73911-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="73911-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="73911-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/participants/invite
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
          "id": "278405a3-f568-4b3e-b684-009193463064",
          "displayName": "string"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="73911-152">C#</span><span class="sxs-lookup"><span data-stu-id="73911-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73911-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73911-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73911-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73911-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73911-155">Java</span><span class="sxs-lookup"><span data-stu-id="73911-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="73911-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="73911-156">Response</span></span>

> <span data-ttu-id="73911-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73911-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "278405a3-f568-4b3e-b684-009193463064",
          "displayName": "string"
        },
        "application": null,
        "device": null,
        "phone": null
      }
    }
  ]
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="73911-159">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="73911-159">Notification - operation completed</span></span>

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
                        "displayName": "string"
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

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="73911-160">Notificação - lista atualizada com o participante adicionado</span><span class="sxs-lookup"><span data-stu-id="73911-160">Notification - roster updated with participant added</span></span>

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
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "application":{
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"278405a3-f568-4b3e-b684-009193463064"
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

### <a name="example-2-invite-multiple-participants-to-an-existing-group-call"></a><span data-ttu-id="73911-161">Exemplo 2: Convidar vários participantes para uma chamada de grupo existente</span><span class="sxs-lookup"><span data-stu-id="73911-161">Example 2: Invite multiple participants to an existing group call</span></span>

> <span data-ttu-id="73911-162">**Observação:** a chamada de grupo existente deve ter um [chatInfo válido.](../resources/chatInfo.md)</span><span class="sxs-lookup"><span data-stu-id="73911-162">**Note**: The existing group call must have a valid [chatInfo](../resources/chatInfo.md).</span></span> <span data-ttu-id="73911-163">Há suporte para até cinco participantes.</span><span class="sxs-lookup"><span data-stu-id="73911-163">Inviting up to 5 participants is supported.</span></span>

##### <a name="request"></a><span data-ttu-id="73911-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73911-164">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="73911-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="73911-165">HTTP</span></span>](#tab/http)
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
          "displayName": "string"
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
          "displayName": "string"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="73911-166">C#</span><span class="sxs-lookup"><span data-stu-id="73911-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-multiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73911-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73911-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-multiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73911-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73911-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-multiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73911-169">Java</span><span class="sxs-lookup"><span data-stu-id="73911-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-invite-multiple-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="73911-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="73911-170">Response</span></span>

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
         "replacesCallId":null,
         "identity":{
            "user":{
              "@odata.type": "#microsoft.graph.identity",
               "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
               "displayName": "string"
            },
            "application":null,
            "device":null,
            "phone":null
         }
      },
      {
         "endpointType":null,
         "replacesCallId":null,
         "identity":{
            "user":{
               "@odata.type": "#microsoft.graph.identity",
               "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
               "displayName": "string"
            },
            "application":null,
            "device":null,
            "phone":null
         }
      }
   ]
}

```
##### <a name="notification---operation-completed"></a><span data-ttu-id="73911-171">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="73911-171">Notification - operation completed</span></span>
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
                "@odata.type": "#microsoft.graph.identity",
                "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                "displayName": "string"
              }
            }
          },
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "@odata.type": "#microsoft.graph.identity",
                "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
                "displayName": "string"
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
##### <a name="notification---roster-updated-with-participants-added"></a><span data-ttu-id="73911-172">Notificação - lista atualizada com participantes adicionados</span><span class="sxs-lookup"><span data-stu-id="73911-172">Notification - roster updated with participants added</span></span>
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
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe"
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
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "@odata.type": "#microsoft.graph.identity",
                "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
                "displayName": "string"
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

### <a name="example-3-invite-participants-to-a-an-existing-group-call-replacing-an-existing-peer-to-peer-call"></a><span data-ttu-id="73911-173">Exemplo 3: Convidar participantes para uma chamada de grupo existente, substituindo uma chamada ponto a ponto existente</span><span class="sxs-lookup"><span data-stu-id="73911-173">Example 3: Invite participants to a an existing group call, replacing an existing Peer-to-Peer call</span></span>


<span data-ttu-id="73911-174">A API de convite dá suporte a apenas um participante ao substituir uma chamada ponto a ponto existente.</span><span class="sxs-lookup"><span data-stu-id="73911-174">The invite API supports only one participant when replacing an existing peer-to-peer call.</span></span> <span data-ttu-id="73911-175">Quando vários participantes são fornecidos no corpo da solicitação, somente o primeiro participante será lido e o restante dos participantes será ignorado.</span><span class="sxs-lookup"><span data-stu-id="73911-175">When multiple participants are provided in the request body, only the first participant will be read and the rest of the participants will be ignored.</span></span>


> <span data-ttu-id="73911-176">**Observação:** A API de convite dá suporte a apenas um participante `replacesCallId` quando fornecido.</span><span class="sxs-lookup"><span data-stu-id="73911-176">**Note:** The invite API supports only one participant when `replacesCallId` is provided.</span></span> 
> <span data-ttu-id="73911-177">Para obter detalhes sobre como usar para substituir uma chamada ponto a ponto existente, consulte `replacesCallId` [invitationParticipantInfo](../resources/invitationparticipantinfo.md).</span><span class="sxs-lookup"><span data-stu-id="73911-177">For  details about using `replacesCallId` to replace an existing peer-to-peer call, see [invitationParticipantInfo](../resources/invitationparticipantinfo.md).</span></span>

##### <a name="request"></a><span data-ttu-id="73911-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73911-178">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="73911-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="73911-179">HTTP</span></span>](#tab/http)
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
          "displayName": "string"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="73911-180">C#</span><span class="sxs-lookup"><span data-stu-id="73911-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-existing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73911-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73911-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-existing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73911-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73911-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-existing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73911-183">Java</span><span class="sxs-lookup"><span data-stu-id="73911-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-invite-existing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="73911-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="73911-184">Response</span></span>

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
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          "displayName": "Participant"
        },
        "application": null,
        "device": null,
        "phone": null
      }
    }
  ]
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="73911-185">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="73911-185">Notification - operation completed</span></span>

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
                        "displayName": "string"
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

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="73911-186">Notificação - lista atualizada com o participante adicionado</span><span class="sxs-lookup"><span data-stu-id="73911-186">Notification - roster updated with participant added</span></span>

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
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "user":{ 
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                        "displayName": "string"
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

><span data-ttu-id="73911-187">**Observação:** Com um status "concluído", você pode esperar receber notificações sobre como sua chamada ponto a ponto original foi encerrada e excluída.</span><span class="sxs-lookup"><span data-stu-id="73911-187">**Note:** With a "completed" status, you can expect to receive notifications on how your original peer-to-peer call has been terminated and deleted.</span></span>

### <a name="example-4-invite-one-pstn-participant-to-an-existing-group-call"></a><span data-ttu-id="73911-188">Exemplo 4: Convidar um participante PSTN para uma chamada de grupo existente</span><span class="sxs-lookup"><span data-stu-id="73911-188">Example 4: Invite one PSTN participant to an existing group call</span></span>

<span data-ttu-id="73911-189">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="73911-189">This call requires an application instance with a PSTN number assigned.</span></span>

#### <a name="step-1-create-application-instance"></a><span data-ttu-id="73911-190">Etapa 1: Criar instância de aplicativo</span><span class="sxs-lookup"><span data-stu-id="73911-190">Step 1: Create application instance</span></span>
<span data-ttu-id="73911-191">Usando credenciais de administrador de locatários, chame os cmdlets a seguir no PowerShell remoto do locatário para criar a instância do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="73911-191">Using tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to create the application instance.</span></span> <span data-ttu-id="73911-192">Para obter mais informações, [consulte New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) e [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="73911-192">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <UPN> -DisplayName <DisplayName> -ApplicationId <AppId>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
#### <a name="step-2-assign-microsoft-365-licenses"></a><span data-ttu-id="73911-193">Etapa 2: Atribuir licenças do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="73911-193">Step 2: Assign Microsoft 365 licenses</span></span>
1. <span data-ttu-id="73911-194">Use as credenciais de administrador de locatários para entrar e acessar a guia https://admin.microsoft.com/ **Usuários -> Usuários ativos.**</span><span class="sxs-lookup"><span data-stu-id="73911-194">Use tenant admin credentials to sign in to https://admin.microsoft.com/ and go to the **Users -> Active users** tab.</span></span>
2. <span data-ttu-id="73911-195">Selecione a instância do aplicativo, atribua o Plano de Chamadas Domésticas e Internacionais do **Microsoft 365** e o Sistema de Telefonia do **Microsoft 365 -** Licenças de Usuário Virtual e clique em Salvar **alterações.**</span><span class="sxs-lookup"><span data-stu-id="73911-195">Select the application instance, assign **Microsoft 365 Domestic and International Calling Plan** and **Microsoft 365 Phone System - Virtual User** licenses, and click **Save changes**.</span></span> <span data-ttu-id="73911-196">Se as licenças necessárias não estão disponíveis no locatário, você pode obter-as na guia Cobrança **-> serviços de** compra.</span><span class="sxs-lookup"><span data-stu-id="73911-196">If the required licenses are not available in the tenant, you can get them from the **Billing -> Purchase services** tab.</span></span>
#### <a name="step-3-acquire-pstn-number"></a><span data-ttu-id="73911-197">Etapa 3: Adquirir número PSTN</span><span class="sxs-lookup"><span data-stu-id="73911-197">Step 3: Acquire PSTN number</span></span>
1. <span data-ttu-id="73911-198">Use as credenciais de administrador de locatários para entrar e clique na guia https://admin.teams.microsoft.com/ **Portal** herddo no painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="73911-198">Use tenant admin credentials to sign in to https://admin.teams.microsoft.com/ and click the **Legacy portal** tab on the left panel.</span></span>
2. <span data-ttu-id="73911-199">Na nova página, vá para a **guia de números de telefone > voz.**</span><span class="sxs-lookup"><span data-stu-id="73911-199">In the new page, go to the **voice -> phone numbers** tab.</span></span>
3. <span data-ttu-id="73911-200">Clique no botão, selecione Novos Números de Serviço e vá para a página Adicionar **+** **novos números de** serviço. </span><span class="sxs-lookup"><span data-stu-id="73911-200">Click the **+** button, select **New Service Numbers**, and go to the **Add new service numbers** page.</span></span>
4. <span data-ttu-id="73911-201">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span><span class="sxs-lookup"><span data-stu-id="73911-201">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span></span> <span data-ttu-id="73911-202">Clique **em adquirir números.**</span><span class="sxs-lookup"><span data-stu-id="73911-202">Click **acquire numbers**.</span></span> <span data-ttu-id="73911-203">O número recém-adquirido será aparecer na guia **números de** telefone.</span><span class="sxs-lookup"><span data-stu-id="73911-203">The newly acquired number will show on  the **phone numbers** tab.</span></span>
#### <a name="step-4-assign-pstn-number-to-application-instance"></a><span data-ttu-id="73911-204">Etapa 4: Atribuir número PSTN à instância do aplicativo</span><span class="sxs-lookup"><span data-stu-id="73911-204">Step 4: Assign PSTN number to application instance</span></span>
<span data-ttu-id="73911-205">Com credenciais de administrador de locatários, chame os cmdlets a seguir no PowerShell remoto do locatário para atribuir o número PSTN à instância do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="73911-205">With tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to assign the PSTN number to the application instance.</span></span> <span data-ttu-id="73911-206">Para obter mais informações, consulte [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) e [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="73911-206">For more information, see [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <UPN> -TelephoneNumber <TelephoneNumber>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```

#### <a name="request"></a><span data-ttu-id="73911-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73911-207">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "participant-invite"
}-->
```http
POST /communications/calls/{id}/participants/invite
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

#### <a name="response"></a><span data-ttu-id="73911-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="73911-208">Response</span></span>

> <span data-ttu-id="73911-p114">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73911-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="notification---operation-completed"></a><span data-ttu-id="73911-211">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="73911-211">Notification - operation completed</span></span>

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

#### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="73911-212">Notificação - lista atualizada com o participante adicionado</span><span class="sxs-lookup"><span data-stu-id="73911-212">Notification - roster updated with participant added</span></span>

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

><span data-ttu-id="73911-213">**Observação:** Com um status, você pode esperar receber notificações sobre como sua chamada ponto a ponto original foi encerrada `completed` e excluída.</span><span class="sxs-lookup"><span data-stu-id="73911-213">**Note:** With a `completed` status, you can expect to receive notifications about how your original peer-to-peer call has been terminated and deleted.</span></span>

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

