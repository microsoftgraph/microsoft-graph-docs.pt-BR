---
title: Obter chamada
description: Recupere as propriedades e os relacionamentos de um objeto de chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 49998005ef65fe132dbc3ff230ea40d25de06b8d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440819"
---
# <a name="get-call"></a><span data-ttu-id="09a47-103">Obter chamada</span><span class="sxs-lookup"><span data-stu-id="09a47-103">Get call</span></span>

<span data-ttu-id="09a47-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="09a47-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09a47-105">Recupere as propriedades e os relacionamentos de um objeto de chamada.</span><span class="sxs-lookup"><span data-stu-id="09a47-105">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="09a47-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="09a47-106">Permissions</span></span>
<span data-ttu-id="09a47-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09a47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09a47-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09a47-109">Permission type</span></span> | <span data-ttu-id="09a47-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09a47-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="09a47-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09a47-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="09a47-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09a47-112">Not Supported.</span></span>                         |
| <span data-ttu-id="09a47-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09a47-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09a47-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09a47-114">Not Supported.</span></span>                         |
| <span data-ttu-id="09a47-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09a47-115">Application</span></span>                            | <span data-ttu-id="09a47-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="09a47-116">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="09a47-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09a47-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /communications/calls/{id}
```
> <span data-ttu-id="09a47-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="09a47-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="09a47-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="09a47-119">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="09a47-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="09a47-120">Optional query parameters</span></span>
<span data-ttu-id="09a47-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="09a47-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09a47-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09a47-122">Request headers</span></span>
| <span data-ttu-id="09a47-123">Nome</span><span class="sxs-lookup"><span data-stu-id="09a47-123">Name</span></span>          | <span data-ttu-id="09a47-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="09a47-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="09a47-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="09a47-125">Authorization</span></span> | <span data-ttu-id="09a47-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09a47-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09a47-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09a47-128">Request body</span></span>
<span data-ttu-id="09a47-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09a47-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09a47-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="09a47-130">Response</span></span>
<span data-ttu-id="09a47-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Call](../resources/call.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09a47-131">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="09a47-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="09a47-132">Examples</span></span>

### <a name="example-1-getting-a-peer-to-peer-call"></a><span data-ttu-id="09a47-133">Exemplo 1: obtendo uma chamada ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="09a47-133">Example 1: Getting a Peer-to-Peer call</span></span>

##### <a name="request"></a><span data-ttu-id="09a47-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09a47-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="09a47-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="09a47-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/{id}
```
# <a name="c"></a>[<span data-ttu-id="09a47-136">C#</span><span class="sxs-lookup"><span data-stu-id="09a47-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09a47-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09a47-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09a47-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09a47-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="09a47-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="09a47-139">Response</span></span>

> <span data-ttu-id="09a47-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09a47-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "established",
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
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
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
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "meetingCapability": null,
  "toneInfo": null
}
```
### <a name="example-2-getting-a-group-call"></a><span data-ttu-id="09a47-142">Exemplo 2: obtendo uma chamada de grupo</span><span class="sxs-lookup"><span data-stu-id="09a47-142">Example 2: Getting a group call</span></span>

##### <a name="request"></a><span data-ttu-id="09a47-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09a47-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="09a47-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="09a47-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
```
# <a name="c"></a>[<span data-ttu-id="09a47-145">C#</span><span class="sxs-lookup"><span data-stu-id="09a47-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09a47-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09a47-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09a47-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09a47-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="09a47-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="09a47-148">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": "true",
  "@odata.type": "microsoft.graph.call"
}-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "established",
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
        "displayName": null
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
  "subject": null,
  "resultInfo": null,
  "answeredBy": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
