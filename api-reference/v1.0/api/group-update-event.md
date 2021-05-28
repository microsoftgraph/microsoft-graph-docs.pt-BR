---
title: Atualizar evento
description: Atualize um objeto event.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0e201980eb74c17d8512e9f98d7a34aa95b20139
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681001"
---
# <a name="update-event"></a><span data-ttu-id="b447f-103">Atualizar evento</span><span class="sxs-lookup"><span data-stu-id="b447f-103">Update event</span></span>

<span data-ttu-id="b447f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b447f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b447f-105">Atualize um objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="b447f-105">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b447f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b447f-106">Permissions</span></span>
<span data-ttu-id="b447f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b447f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b447f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b447f-109">Permission type</span></span>      | <span data-ttu-id="b447f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b447f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b447f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b447f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b447f-112">Calendars.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b447f-112">Calendars.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b447f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b447f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b447f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b447f-114">Not supported.</span></span>    |
|<span data-ttu-id="b447f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b447f-115">Application</span></span> | <span data-ttu-id="b447f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b447f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b447f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b447f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b447f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b447f-118">Request headers</span></span>
| <span data-ttu-id="b447f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b447f-119">Name</span></span>       | <span data-ttu-id="b447f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b447f-120">Type</span></span> | <span data-ttu-id="b447f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b447f-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b447f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b447f-122">Authorization</span></span>  | <span data-ttu-id="b447f-123">string</span><span class="sxs-lookup"><span data-stu-id="b447f-123">string</span></span>  | <span data-ttu-id="b447f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b447f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b447f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b447f-126">Request body</span></span>
<span data-ttu-id="b447f-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b447f-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="b447f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b447f-130">Response</span></span>
<span data-ttu-id="b447f-131">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="b447f-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b447f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b447f-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b447f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b447f-133">Request</span></span>
<span data-ttu-id="b447f-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b447f-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b447f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b447f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["01d4ee64-15ce-491e-bad1-b91aa3223df4", "AAMkADZlAAAAABERAAA="],
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/01d4ee64-15ce-491e-bad1-b91aa3223df4/calendar/events/AAMkADZlAAAAABERAAA=
Content-type: application/json

{ 
  "location":{
      "displayName":"Conf Room 2"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="b447f-136">C#</span><span class="sxs-lookup"><span data-stu-id="b447f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b447f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b447f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b447f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b447f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b447f-139">Java</span><span class="sxs-lookup"><span data-stu-id="b447f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b447f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b447f-140">Response</span></span>
<span data-ttu-id="b447f-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b447f-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.event",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('01d4ee64-15ce-491e-bad1-b91aa3223df4')/calendar/events/$entity",
    "@odata.etag": "W/\"Na8DfbsBGUG8JeyvlwNi5wAAHMKyZg==\"",
    "id": "AAMkADZlAAAAABERAAA=",
    "createdDateTime": "2019-04-06T13:19:09.2517612Z",
    "lastModifiedDateTime": "2019-05-20T00:14:51.2677891Z",
    "changeKey": "Na8DfbsBGUG8JeyvlwNi5wAAHMKyZg==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200E00074C5B7101A82E00800000000B7CA7D517BECD40100000000000000001000000011E38F935AD4FF41BDAB12A2F3E15103",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Planogram Training",
    "bodyPreview": "Need more help with visual merchandising?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADZlAAAAABERAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\n<div>Need more help with visual merchandising?\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-04-16T22:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2019-04-16T23:00:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "Conf Room 2",
        "locationType": "default",
        "uniqueId": "Conf Room 2",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Conf Room 2",
            "locationType": "default",
            "uniqueId": "Conf Room 2",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "accepted",
                "time": "2019-04-06T13:19:12.1060982Z"
            },
            "emailAddress": {
                "name": "Johanna Lorenz",
                "address": "JohannaL@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Retail",
                "address": "Retail@contoso.onmicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Alex Wilber",
                "address": "AlexW@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Nestor Wilke",
                "address": "NestorW@contoso.OnMicrosoft.com"
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
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

