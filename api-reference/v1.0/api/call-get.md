---
title: Obter chamada
description: Recupere as propriedades e os relacionamentos de um objeto de chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: c66dd25ea1f58fec94dc32ad4e195802583cfe11
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518718"
---
# <a name="get-call"></a><span data-ttu-id="e3b14-103">Obter chamada</span><span class="sxs-lookup"><span data-stu-id="e3b14-103">Get call</span></span>

<span data-ttu-id="e3b14-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3b14-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3b14-105">Recupere as propriedades e os relacionamentos de um objeto de chamada.</span><span class="sxs-lookup"><span data-stu-id="e3b14-105">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3b14-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3b14-106">Permissions</span></span>
<span data-ttu-id="e3b14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3b14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3b14-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3b14-109">Permission type</span></span> | <span data-ttu-id="e3b14-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3b14-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="e3b14-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3b14-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3b14-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3b14-112">Not Supported.</span></span>                         |
| <span data-ttu-id="e3b14-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3b14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3b14-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3b14-114">Not Supported.</span></span>                         |
| <span data-ttu-id="e3b14-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3b14-115">Application</span></span>                            | <span data-ttu-id="e3b14-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3b14-116">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="e3b14-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3b14-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /communications/calls/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3b14-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e3b14-118">Optional query parameters</span></span>
<span data-ttu-id="e3b14-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e3b14-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3b14-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3b14-120">Request headers</span></span>
| <span data-ttu-id="e3b14-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e3b14-121">Name</span></span>          | <span data-ttu-id="e3b14-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3b14-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e3b14-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3b14-123">Authorization</span></span> | <span data-ttu-id="e3b14-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3b14-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3b14-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3b14-126">Request body</span></span>
<span data-ttu-id="e3b14-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3b14-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3b14-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3b14-128">Response</span></span>
<span data-ttu-id="e3b14-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Call](../resources/call.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3b14-129">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3b14-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e3b14-130">Examples</span></span>

### <a name="example-1-getting-a-peer-to-peer-call"></a><span data-ttu-id="e3b14-131">Exemplo 1: obtendo uma chamada ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="e3b14-131">Example 1: Getting a Peer-to-Peer call</span></span>

##### <a name="request"></a><span data-ttu-id="e3b14-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3b14-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e3b14-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3b14-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/{id}
```
# <a name="c"></a>[<span data-ttu-id="e3b14-134">C#</span><span class="sxs-lookup"><span data-stu-id="e3b14-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3b14-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3b14-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3b14-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3b14-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3b14-137">Java</span><span class="sxs-lookup"><span data-stu-id="e3b14-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e3b14-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3b14-138">Response</span></span>

> <span data-ttu-id="e3b14-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3b14-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      }
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/calls/$entity",
  "subject": null,
  "ringingTimeoutInSeconds": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "toneInfo": null
}
```
### <a name="example-2-getting-a-group-call"></a><span data-ttu-id="e3b14-141">Exemplo 2: obtendo uma chamada de grupo</span><span class="sxs-lookup"><span data-stu-id="e3b14-141">Example 2: Getting a group call</span></span>

##### <a name="request"></a><span data-ttu-id="e3b14-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3b14-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e3b14-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3b14-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
```
# <a name="c"></a>[<span data-ttu-id="e3b14-144">C#</span><span class="sxs-lookup"><span data-stu-id="e3b14-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3b14-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3b14-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3b14-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3b14-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3b14-147">Java</span><span class="sxs-lookup"><span data-stu-id="e3b14-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e3b14-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3b14-148">Response</span></span>

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
        "displayName": null
      }
    },
    "allowConversationWithoutHost": true
  },
  "myParticipantId": "05491616-385f-44a8-9974-18cc5f9933c1",
  "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/calls/$entity",
  "ringingTimeoutInSeconds": null,
  "subject": null,
  "resultInfo": null,
  "answeredBy": null,
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
