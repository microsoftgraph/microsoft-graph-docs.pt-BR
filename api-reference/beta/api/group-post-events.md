---
title: Criar evento
description: Use esta API para criar um novo evento.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9477d63235ee6b9cf5137ac899e3decffadbf1c3
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420655"
---
# <a name="create-event"></a><span data-ttu-id="9ff86-103">Criar evento</span><span class="sxs-lookup"><span data-stu-id="9ff86-103">Create event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ff86-104">Use esta API para criar um novo [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="9ff86-104">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ff86-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ff86-105">Permissions</span></span>
<span data-ttu-id="9ff86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ff86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ff86-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ff86-108">Permission type</span></span>      | <span data-ttu-id="9ff86-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ff86-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ff86-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ff86-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9ff86-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ff86-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9ff86-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ff86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ff86-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ff86-113">Not supported.</span></span>    |
|<span data-ttu-id="9ff86-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ff86-114">Application</span></span> | <span data-ttu-id="9ff86-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ff86-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ff86-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ff86-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="9ff86-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ff86-117">Request headers</span></span>
| <span data-ttu-id="9ff86-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ff86-118">Header</span></span>       | <span data-ttu-id="9ff86-119">Valor</span><span class="sxs-lookup"><span data-stu-id="9ff86-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ff86-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ff86-120">Authorization</span></span>  | <span data-ttu-id="9ff86-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ff86-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9ff86-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ff86-123">Request body</span></span>
<span data-ttu-id="9ff86-124">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="9ff86-124">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9ff86-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ff86-125">Response</span></span>
<span data-ttu-id="9ff86-126">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ff86-126">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ff86-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ff86-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9ff86-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ff86-128">Request</span></span>
<span data-ttu-id="9ff86-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ff86-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9ff86-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ff86-130">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ff86-131">C#</span><span class="sxs-lookup"><span data-stu-id="9ff86-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ff86-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ff86-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ff86-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9ff86-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="9ff86-134">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="9ff86-134">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="9ff86-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ff86-135">Response</span></span>
<span data-ttu-id="9ff86-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9ff86-136">The following is an example of the response.</span></span>
><span data-ttu-id="9ff86-137">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9ff86-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9ff86-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ff86-138">All the properties will be returned from an actual call.</span></span>
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
