---
title: Criar evento
description: Use esta API para criar um novo evento.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7298cd8d0e9ecdb5773f524f248fef85d0a0a540
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041222"
---
# <a name="create-event"></a><span data-ttu-id="2ba34-103">Criar evento</span><span class="sxs-lookup"><span data-stu-id="2ba34-103">Create event</span></span>

<span data-ttu-id="2ba34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ba34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ba34-105">Use esta API para criar um novo [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="2ba34-105">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2ba34-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ba34-106">Permissions</span></span>
<span data-ttu-id="2ba34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ba34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ba34-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ba34-109">Permission type</span></span>      | <span data-ttu-id="2ba34-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ba34-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ba34-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ba34-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ba34-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ba34-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2ba34-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ba34-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ba34-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ba34-114">Not supported.</span></span>    |
|<span data-ttu-id="2ba34-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ba34-115">Application</span></span> | <span data-ttu-id="2ba34-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ba34-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ba34-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ba34-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="2ba34-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ba34-118">Request headers</span></span>
| <span data-ttu-id="2ba34-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ba34-119">Header</span></span>       | <span data-ttu-id="2ba34-120">Valor</span><span class="sxs-lookup"><span data-stu-id="2ba34-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2ba34-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ba34-121">Authorization</span></span>  | <span data-ttu-id="2ba34-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ba34-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2ba34-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ba34-124">Request body</span></span>
<span data-ttu-id="2ba34-125">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="2ba34-125">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2ba34-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ba34-126">Response</span></span>
<span data-ttu-id="2ba34-127">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ba34-127">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ba34-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ba34-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2ba34-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ba34-129">Request</span></span>
<span data-ttu-id="2ba34-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ba34-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ba34-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ba34-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["01d4ee64-15ce-491e-bad1-b91aa3223df4"],
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/01d4ee64-15ce-491e-bad1-b91aa3223df4/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
  },
  "start": {
      "dateTime": "2019-06-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-06-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"adelev@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="2ba34-132">C#</span><span class="sxs-lookup"><span data-stu-id="2ba34-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ba34-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ba34-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ba34-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ba34-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ba34-135">Java</span><span class="sxs-lookup"><span data-stu-id="2ba34-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2ba34-136">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="2ba34-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="2ba34-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ba34-137">Response</span></span>
<span data-ttu-id="2ba34-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2ba34-138">The following is an example of the response.</span></span>
><span data-ttu-id="2ba34-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2ba34-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('01d4ee64-15ce-491e-bad1-b91aa3223df4')/events/$entity",
    "@odata.etag": "W/\"Na8DfbsBGUG8JeyvlwNi5wAAHMK0mg==\"",
    "id": "AAMkADZ_XA2LnAAAcwiSBAAA=",
    "createdDateTime": "2019-05-20T02:14:32.7419058Z",
    "lastModifiedDateTime": "2019-05-20T02:14:33.342409Z",
    "changeKey": "Na8DfbsBGUG8JeyvlwNi5wAAHMK0mg==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "uid": "040000008200E00074C5B7101A82E00800000000DE7664C3B10ED501000000000000000010000000EC2760BC8BC4AF4BAC1C9730C3E534AC",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does late morning work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isDraft": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADZ%2BXA2LnAAAcwiSBAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes late morning work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-06-15T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-06-15T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueId": "Harry's Bar",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Adele Vance",
                "address": "adelev@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Retail",
            "address": "Retail@contoso.onmicrosoft.com"
        }
    }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


