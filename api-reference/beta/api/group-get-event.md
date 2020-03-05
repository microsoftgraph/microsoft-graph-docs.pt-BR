---
title: Obter evento
description: Obter um objeto event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e2a6f08c4e00b3d9a4fe2e4032b3b3477c9fe343
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419923"
---
# <a name="get-event"></a><span data-ttu-id="1fd27-103">Obter evento</span><span class="sxs-lookup"><span data-stu-id="1fd27-103">Get event</span></span>

<span data-ttu-id="1fd27-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1fd27-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fd27-105">Obter um objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="1fd27-105">Get an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fd27-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1fd27-106">Permissions</span></span>
<span data-ttu-id="1fd27-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fd27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fd27-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fd27-109">Permission type</span></span>      | <span data-ttu-id="1fd27-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1fd27-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fd27-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fd27-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1fd27-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fd27-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1fd27-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fd27-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fd27-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fd27-114">Not supported.</span></span>    |
|<span data-ttu-id="1fd27-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fd27-115">Application</span></span> | <span data-ttu-id="1fd27-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fd27-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fd27-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fd27-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}
GET /groups/{id}/calendar/events/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1fd27-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1fd27-118">Optional query parameters</span></span>
<span data-ttu-id="1fd27-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1fd27-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1fd27-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fd27-120">Request headers</span></span>
| <span data-ttu-id="1fd27-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1fd27-121">Name</span></span>       | <span data-ttu-id="1fd27-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fd27-122">Type</span></span> | <span data-ttu-id="1fd27-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fd27-123">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="1fd27-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fd27-124">Authorization</span></span>  | <span data-ttu-id="1fd27-125">string</span><span class="sxs-lookup"><span data-stu-id="1fd27-125">string</span></span> | <span data-ttu-id="1fd27-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fd27-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1fd27-128">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="1fd27-128">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="1fd27-129">string</span><span class="sxs-lookup"><span data-stu-id="1fd27-129">string</span></span> | <span data-ttu-id="1fd27-130">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="1fd27-130">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="1fd27-131">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="1fd27-131">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="1fd27-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1fd27-132">Optional.</span></span> |
| <span data-ttu-id="1fd27-133">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="1fd27-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="1fd27-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1fd27-134">string</span></span> | <span data-ttu-id="1fd27-135">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="1fd27-135">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="1fd27-136">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="1fd27-136">Values can be "text" or "html".</span></span> <span data-ttu-id="1fd27-137">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="1fd27-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="1fd27-138">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="1fd27-138">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="1fd27-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1fd27-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fd27-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fd27-140">Request body</span></span>
<span data-ttu-id="1fd27-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1fd27-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fd27-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fd27-142">Response</span></span>
<span data-ttu-id="1fd27-143">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fd27-143">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fd27-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1fd27-144">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1fd27-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fd27-145">Request</span></span>
<span data-ttu-id="1fd27-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fd27-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1fd27-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fd27-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_event"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```
# <a name="c"></a>[<span data-ttu-id="1fd27-148">C#</span><span class="sxs-lookup"><span data-stu-id="1fd27-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fd27-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fd27-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fd27-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fd27-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1fd27-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fd27-151">Response</span></span>
<span data-ttu-id="1fd27-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1fd27-152">The following is an example of the response.</span></span>
><span data-ttu-id="1fd27-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1fd27-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1728

{
    "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==",
    "createdDateTime": "2017-07-31T18:58:31.011909Z",
    "lastModifiedDateTime": "2017-07-31T18:58:35.418473Z",
    "changeKey": "xPZF2y46pEiVBni87OnrpgAAAAAJTg==",
    "categories": [],
    "originalStartTimeZone": "Eastern Standard Time",
    "originalEndTimeZone": "Eastern Standard Time",
    "uid": "040000008200E00074C5B7101A82E00800000000B23663002F0AD301000000000000000010000000B7C936D4C2FEC749824EE24B2FD7DA62",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Continuing Education Sync",
    "bodyPreview": "Higher Education Planning.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "seriesMaster",
    "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA%3D%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Higher Education Planning.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2017-08-15T14:30:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2017-08-15T15:30:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "HR Taskforce / Benefits"
    },
    "recurrence": {
        "pattern": {
            "type": "weekly",
            "interval": 1,
            "month": 0,
            "dayOfMonth": 0,
            "daysOfWeek": [
                "tuesday",
                "thursday"
            ],
            "firstDayOfWeek": "sunday",
            "index": "first"
        },
        "range": {
            "type": "noEnd",
            "startDate": "2017-08-15",
            "endDate": "0001-01-01",
            "recurrenceTimeZone": "Eastern Standard Time",
            "numberOfOccurrences": 0
        }
    },
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "accepted",
                "time": "2017-07-31T18:58:34.3298022Z"
            },
            "emailAddress": {
                "name": "Lidia Holloway",
                "address": "LidiaH@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "HR Taskforce",
                "address": "HRTaskforce@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Diego Siciliani",
                "address": "DiegoS@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Johanna Lorenz",
                "address": "JohannaL@contoso.com"
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
                "address": "MeganB@contoso.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "HR Taskforce",
            "address": "HRTaskforce@contoso.com"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
