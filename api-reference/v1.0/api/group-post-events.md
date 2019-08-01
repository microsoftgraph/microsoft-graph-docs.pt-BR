---
title: Criar evento
description: Use esta API para criar um novo evento.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3328e22eef7cf5434ac5e20791e4083e188f5bae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016277"
---
# <a name="create-event"></a><span data-ttu-id="0dae9-103">Criar evento</span><span class="sxs-lookup"><span data-stu-id="0dae9-103">Create event</span></span>
<span data-ttu-id="0dae9-104">Use esta API para criar um novo [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="0dae9-104">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0dae9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0dae9-105">Permissions</span></span>
<span data-ttu-id="0dae9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0dae9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0dae9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0dae9-108">Permission type</span></span>      | <span data-ttu-id="0dae9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0dae9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0dae9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0dae9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0dae9-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dae9-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0dae9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0dae9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0dae9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0dae9-113">Not supported.</span></span>    |
|<span data-ttu-id="0dae9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0dae9-114">Application</span></span> | <span data-ttu-id="0dae9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0dae9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0dae9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0dae9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="0dae9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0dae9-117">Request headers</span></span>
| <span data-ttu-id="0dae9-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0dae9-118">Header</span></span>       | <span data-ttu-id="0dae9-119">Valor</span><span class="sxs-lookup"><span data-stu-id="0dae9-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0dae9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0dae9-120">Authorization</span></span>  | <span data-ttu-id="0dae9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0dae9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0dae9-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0dae9-123">Request body</span></span>
<span data-ttu-id="0dae9-124">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="0dae9-124">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0dae9-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="0dae9-125">Response</span></span>
<span data-ttu-id="0dae9-126">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0dae9-126">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0dae9-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0dae9-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0dae9-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0dae9-128">Request</span></span>
<span data-ttu-id="0dae9-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0dae9-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0dae9-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0dae9-130">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["01d4ee64-15ce-491e-bad1-b91aa3223df4"],
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/01d4ee64-15ce-491e-bad1-b91aa3223df4/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
  },
  "start": {
      "dateTime": "2019-06-16T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-06-16T14:00:00",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0dae9-131">C#</span><span class="sxs-lookup"><span data-stu-id="0dae9-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0dae9-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="0dae9-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0dae9-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0dae9-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0dae9-134">Java</span><span class="sxs-lookup"><span data-stu-id="0dae9-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0dae9-135">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="0dae9-135">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="0dae9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0dae9-136">Response</span></span>
<span data-ttu-id="0dae9-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0dae9-137">The following is an example of the response.</span></span>
><span data-ttu-id="0dae9-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0dae9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('01d4ee64-15ce-491e-bad1-b91aa3223df4')/events/$entity",
    "@odata.etag": "W/\"Na8DfbsBGUG8JeyvlwNi5wAAHMK0vA==\"",
    "id": "AAMkADZlEZQbwl7K_XA2LnAAAcwiSBAAA=ZQbwl7K_XA2LnAAAcwiSDAAA=",
    "createdDateTime": "2019-05-20T02:20:45.3057043Z",
    "lastModifiedDateTime": "2019-05-20T02:20:45.5639203Z",
    "changeKey": "Na8DfbsBGUG8JeyvlwNi5wAAHMK0vA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200E00074C5B7101A82E008000000005D5775A1B20ED50100000000000000001000000072FA001DBB385A45B6AE65DB0E356105",
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
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADZN9uwEZQbwl7K%2BXA2LnAAAAAAENAAA1rwN9uwEZQbwl7K%2BXA2LnAAAcwiSDAAA%3D&exvsurl=1&path=/calendar/item",
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
        "dateTime": "2019-06-16T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-06-16T14:00:00.0000000",
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
