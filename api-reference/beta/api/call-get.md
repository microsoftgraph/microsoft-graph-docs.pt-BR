---
title: Obter chamada
description: Recupere as propriedades e os relacionamentos de um objeto de chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 12641164d8334a30f5903462497792f00e30dc9c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959728"
---
# <a name="get-call"></a><span data-ttu-id="a61b4-103">Obter chamada</span><span class="sxs-lookup"><span data-stu-id="a61b4-103">Get call</span></span>

<span data-ttu-id="a61b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a61b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a61b4-105">Recupere as propriedades e os relacionamentos de um objeto de chamada.</span><span class="sxs-lookup"><span data-stu-id="a61b4-105">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a61b4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a61b4-106">Permissions</span></span>
<span data-ttu-id="a61b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a61b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a61b4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a61b4-109">Permission type</span></span> | <span data-ttu-id="a61b4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a61b4-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="a61b4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a61b4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a61b4-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a61b4-112">Not Supported.</span></span>                         |
| <span data-ttu-id="a61b4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a61b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a61b4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a61b4-114">Not Supported.</span></span>                         |
| <span data-ttu-id="a61b4-115">Application</span><span class="sxs-lookup"><span data-stu-id="a61b4-115">Application</span></span>                            | <span data-ttu-id="a61b4-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a61b4-116">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="a61b4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a61b4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /communications/calls/{id}
```
> <span data-ttu-id="a61b4-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="a61b4-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="a61b4-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="a61b4-119">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="a61b4-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a61b4-120">Optional query parameters</span></span>
<span data-ttu-id="a61b4-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a61b4-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a61b4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a61b4-122">Request headers</span></span>
| <span data-ttu-id="a61b4-123">Nome</span><span class="sxs-lookup"><span data-stu-id="a61b4-123">Name</span></span>          | <span data-ttu-id="a61b4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a61b4-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a61b4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a61b4-125">Authorization</span></span> | <span data-ttu-id="a61b4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a61b4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a61b4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a61b4-128">Request body</span></span>
<span data-ttu-id="a61b4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a61b4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a61b4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a61b4-130">Response</span></span>
<span data-ttu-id="a61b4-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Call](../resources/call.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a61b4-131">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a61b4-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a61b4-132">Examples</span></span>

### <a name="example-1-getting-a-peer-to-peer-call"></a><span data-ttu-id="a61b4-133">Exemplo 1: obtendo uma chamada ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="a61b4-133">Example 1: Getting a Peer-to-Peer call</span></span>

##### <a name="request"></a><span data-ttu-id="a61b4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a61b4-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a61b4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a61b4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/{id}
```
# <a name="c"></a>[<span data-ttu-id="a61b4-136">C#</span><span class="sxs-lookup"><span data-stu-id="a61b4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a61b4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a61b4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a61b4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a61b4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a61b4-139">Java</span><span class="sxs-lookup"><span data-stu-id="a61b4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a61b4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a61b4-140">Response</span></span>

> <span data-ttu-id="a61b4-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a61b4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "transcription": null,
  "meetingCapability": null,
  "toneInfo": null
}
```
### <a name="example-2-getting-a-group-call"></a><span data-ttu-id="a61b4-143">Exemplo 2: obtendo uma chamada de grupo</span><span class="sxs-lookup"><span data-stu-id="a61b4-143">Example 2: Getting a group call</span></span>

##### <a name="request"></a><span data-ttu-id="a61b4-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a61b4-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a61b4-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="a61b4-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
```
# <a name="c"></a>[<span data-ttu-id="a61b4-146">C#</span><span class="sxs-lookup"><span data-stu-id="a61b4-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a61b4-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a61b4-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a61b4-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a61b4-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a61b4-149">Java</span><span class="sxs-lookup"><span data-stu-id="a61b4-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a61b4-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="a61b4-150">Response</span></span>

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
  "transcription": {
    "@odata.type": "#microsoft.graph.callTranscriptionInfo",
    "state": "inactive",
    "lastModifiedDateTime": "2020-05-28T00:10:54.104318Z"
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


