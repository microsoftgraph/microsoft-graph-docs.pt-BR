---
title: Obter evento
description: Obter um objeto event.
author: dkershaw10
ms.openlocfilehash: d599df555d93459df8d7985dd726d2280b019e68
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307515"
---
# <a name="get-event"></a><span data-ttu-id="ab446-103">Obter evento</span><span class="sxs-lookup"><span data-stu-id="ab446-103">Get event</span></span>
<span data-ttu-id="ab446-104">Obter um objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="ab446-104">Get an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab446-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab446-105">Permissions</span></span>
<span data-ttu-id="ab446-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab446-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab446-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab446-108">Permission type</span></span>      | <span data-ttu-id="ab446-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab446-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab446-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab446-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ab446-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab446-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab446-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab446-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab446-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab446-113">Not supported.</span></span>    |
|<span data-ttu-id="ab446-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab446-114">Application</span></span> | <span data-ttu-id="ab446-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab446-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab446-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab446-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}
GET /groups/{id}/calendar/events/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab446-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab446-117">Optional query parameters</span></span>
<span data-ttu-id="ab446-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab446-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab446-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab446-119">Request headers</span></span>
| <span data-ttu-id="ab446-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ab446-120">Name</span></span>       | <span data-ttu-id="ab446-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab446-121">Type</span></span> | <span data-ttu-id="ab446-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab446-122">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="ab446-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab446-123">Authorization</span></span>  | <span data-ttu-id="ab446-124">string</span><span class="sxs-lookup"><span data-stu-id="ab446-124">string</span></span> | <span data-ttu-id="ab446-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab446-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ab446-127">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="ab446-127">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="ab446-128">string</span><span class="sxs-lookup"><span data-stu-id="ab446-128">string</span></span> | <span data-ttu-id="ab446-129">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="ab446-129">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="ab446-130">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="ab446-130">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="ab446-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ab446-131">Optional.</span></span> |
| <span data-ttu-id="ab446-132">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="ab446-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="ab446-133">string</span><span class="sxs-lookup"><span data-stu-id="ab446-133">string</span></span> | <span data-ttu-id="ab446-134">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="ab446-134">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="ab446-135">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="ab446-135">Values can be "text" or "html".</span></span> <span data-ttu-id="ab446-136">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="ab446-136">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="ab446-137">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="ab446-137">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="ab446-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ab446-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab446-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab446-139">Request body</span></span>
<span data-ttu-id="ab446-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab446-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab446-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab446-141">Response</span></span>
<span data-ttu-id="ab446-142">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab446-142">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab446-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab446-143">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ab446-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab446-144">Request</span></span>
<span data-ttu-id="ab446-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab446-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA=="],
  "name": "get_group_event"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="ab446-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab446-146">Response</span></span>
<span data-ttu-id="ab446-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ab446-147">The following is an example of the response.</span></span>
><span data-ttu-id="ab446-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab446-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "iCalUId": "040000008200E00074C5B7101A82E00800000000B23663002F0AD301000000000000000010000000B7C936D4C2FEC749824EE24B2FD7DA62",
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
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
