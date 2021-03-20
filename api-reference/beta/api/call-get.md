---
title: Obter chamada
description: Recupere as propriedades e as relações de um objeto de chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 035dfff2d7189f67f05de241997391fb86437dce
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948512"
---
# <a name="get-call"></a><span data-ttu-id="1ff8b-103">Obter chamada</span><span class="sxs-lookup"><span data-stu-id="1ff8b-103">Get call</span></span>

<span data-ttu-id="1ff8b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ff8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ff8b-105">Recupere as propriedades e as relações de um objeto de chamada.</span><span class="sxs-lookup"><span data-stu-id="1ff8b-105">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ff8b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1ff8b-106">Permissions</span></span>
<span data-ttu-id="1ff8b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ff8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ff8b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ff8b-109">Permission type</span></span> | <span data-ttu-id="1ff8b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1ff8b-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="1ff8b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ff8b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ff8b-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ff8b-112">Not Supported.</span></span>                         |
| <span data-ttu-id="1ff8b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ff8b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ff8b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ff8b-114">Not Supported.</span></span>                         |
| <span data-ttu-id="1ff8b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ff8b-115">Application</span></span>                            | <span data-ttu-id="1ff8b-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ff8b-116">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="1ff8b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ff8b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /communications/calls/{id}
```
> <span data-ttu-id="1ff8b-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="1ff8b-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="1ff8b-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="1ff8b-119">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="1ff8b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1ff8b-120">Optional query parameters</span></span>
<span data-ttu-id="1ff8b-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1ff8b-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ff8b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ff8b-122">Request headers</span></span>
| <span data-ttu-id="1ff8b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1ff8b-123">Name</span></span>          | <span data-ttu-id="1ff8b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ff8b-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1ff8b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ff8b-125">Authorization</span></span> | <span data-ttu-id="1ff8b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ff8b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ff8b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ff8b-128">Request body</span></span>
<span data-ttu-id="1ff8b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1ff8b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ff8b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ff8b-130">Response</span></span>
<span data-ttu-id="1ff8b-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto de](../resources/call.md) chamada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ff8b-131">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ff8b-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1ff8b-132">Examples</span></span>

### <a name="example-1-getting-a-peer-to-peer-call"></a><span data-ttu-id="1ff8b-133">Exemplo 1: Recebendo uma chamada ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="1ff8b-133">Example 1: Getting a Peer-to-Peer call</span></span>

##### <a name="request"></a><span data-ttu-id="1ff8b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ff8b-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1ff8b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ff8b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call-1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/{id}
```
# <a name="c"></a>[<span data-ttu-id="1ff8b-136">C#</span><span class="sxs-lookup"><span data-stu-id="1ff8b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ff8b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ff8b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ff8b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ff8b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ff8b-139">Java</span><span class="sxs-lookup"><span data-stu-id="1ff8b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-call-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1ff8b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ff8b-140">Response</span></span>

> <span data-ttu-id="1ff8b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ff8b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-getting-a-group-call"></a><span data-ttu-id="1ff8b-143">Exemplo 2: Receber uma chamada de grupo</span><span class="sxs-lookup"><span data-stu-id="1ff8b-143">Example 2: Getting a group call</span></span>

##### <a name="request"></a><span data-ttu-id="1ff8b-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ff8b-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1ff8b-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ff8b-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call-2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
```
# <a name="c"></a>[<span data-ttu-id="1ff8b-146">C#</span><span class="sxs-lookup"><span data-stu-id="1ff8b-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ff8b-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ff8b-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ff8b-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ff8b-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ff8b-149">Java</span><span class="sxs-lookup"><span data-stu-id="1ff8b-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-call-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1ff8b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ff8b-150">Response</span></span>

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


