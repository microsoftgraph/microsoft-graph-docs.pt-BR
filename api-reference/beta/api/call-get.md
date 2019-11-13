---
title: Obter chamada
description: Recupere as propriedades e os relacionamentos de um objeto de chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: dcf71d38535d0e033305e9ed945abf17cee1282a
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302239"
---
# <a name="get-call"></a><span data-ttu-id="fda3b-103">Obter chamada</span><span class="sxs-lookup"><span data-stu-id="fda3b-103">Get call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fda3b-104">Recupere as propriedades e os relacionamentos de um objeto de chamada.</span><span class="sxs-lookup"><span data-stu-id="fda3b-104">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fda3b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fda3b-105">Permissions</span></span>
<span data-ttu-id="fda3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fda3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fda3b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fda3b-108">Permission type</span></span> | <span data-ttu-id="fda3b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fda3b-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="fda3b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fda3b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fda3b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fda3b-111">Not Supported.</span></span>                         |
| <span data-ttu-id="fda3b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fda3b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fda3b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fda3b-113">Not Supported.</span></span>                         |
| <span data-ttu-id="fda3b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fda3b-114">Application</span></span>                            | <span data-ttu-id="fda3b-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fda3b-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="fda3b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fda3b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /communications/calls/{id}
```
> <span data-ttu-id="fda3b-117">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="fda3b-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="fda3b-118">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="fda3b-118">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="fda3b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fda3b-119">Optional query parameters</span></span>
<span data-ttu-id="fda3b-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fda3b-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fda3b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fda3b-121">Request headers</span></span>
| <span data-ttu-id="fda3b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fda3b-122">Name</span></span>          | <span data-ttu-id="fda3b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fda3b-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fda3b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fda3b-124">Authorization</span></span> | <span data-ttu-id="fda3b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fda3b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fda3b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fda3b-127">Request body</span></span>
<span data-ttu-id="fda3b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fda3b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fda3b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fda3b-129">Response</span></span>
<span data-ttu-id="fda3b-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Call](../resources/call.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fda3b-130">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fda3b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fda3b-131">Examples</span></span>

### <a name="example-1-getting-a-peer-to-peer-call"></a><span data-ttu-id="fda3b-132">Exemplo 1: obtendo uma chamada ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="fda3b-132">Example 1: Getting a Peer-to-Peer call</span></span>

##### <a name="request"></a><span data-ttu-id="fda3b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fda3b-133">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fda3b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fda3b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fda3b-135">C#</span><span class="sxs-lookup"><span data-stu-id="fda3b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fda3b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fda3b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fda3b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fda3b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fda3b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fda3b-138">Response</span></span>

> <span data-ttu-id="fda3b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fda3b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "@odata.type": "#microsoft.graph.participantInfo",
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
### <a name="example-2-getting-a-group-call"></a><span data-ttu-id="fda3b-141">Exemplo 2: obtendo uma chamada de grupo</span><span class="sxs-lookup"><span data-stu-id="fda3b-141">Example 2: Getting a group call</span></span>

##### <a name="request"></a><span data-ttu-id="fda3b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fda3b-142">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fda3b-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="fda3b-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fda3b-144">C#</span><span class="sxs-lookup"><span data-stu-id="fda3b-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fda3b-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fda3b-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fda3b-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fda3b-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fda3b-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="fda3b-147">Response</span></span>

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
