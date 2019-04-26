---
title: Listar calendarView
description: Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida, do calendário padrão de um grupo.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 4e3f1c6d7bcb5c68015c60e48f2dc3ef71c9f6c7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329642"
---
# <a name="list-calendarview"></a><span data-ttu-id="85d55-103">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="85d55-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85d55-104">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida, do calendário padrão de um grupo.</span><span class="sxs-lookup"><span data-stu-id="85d55-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="85d55-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="85d55-105">Permissions</span></span>
<span data-ttu-id="85d55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85d55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85d55-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85d55-108">Permission type</span></span>      | <span data-ttu-id="85d55-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85d55-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85d55-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85d55-110">Delegated (work or school account)</span></span> | <span data-ttu-id="85d55-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85d55-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="85d55-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85d55-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85d55-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85d55-113">Not supported.</span></span>    |
|<span data-ttu-id="85d55-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85d55-114">Application</span></span> | <span data-ttu-id="85d55-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85d55-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85d55-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85d55-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="85d55-117">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="85d55-117">Query parameters</span></span>
<span data-ttu-id="85d55-118">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="85d55-118">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="85d55-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="85d55-119">Parameter</span></span>    | <span data-ttu-id="85d55-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="85d55-120">Type</span></span>   |<span data-ttu-id="85d55-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="85d55-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85d55-122">startDateTime</span><span class="sxs-lookup"><span data-stu-id="85d55-122">startDateTime</span></span>|<span data-ttu-id="85d55-123">String</span><span class="sxs-lookup"><span data-stu-id="85d55-123">String</span></span>|<span data-ttu-id="85d55-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="85d55-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="85d55-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="85d55-126">endDateTime</span></span>|<span data-ttu-id="85d55-127">String</span><span class="sxs-lookup"><span data-stu-id="85d55-127">String</span></span>|<span data-ttu-id="85d55-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="85d55-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="85d55-130">Este método também dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="85d55-130">This method also supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85d55-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85d55-131">Request headers</span></span>
| <span data-ttu-id="85d55-132">Nome</span><span class="sxs-lookup"><span data-stu-id="85d55-132">Name</span></span>       | <span data-ttu-id="85d55-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="85d55-133">Type</span></span> | <span data-ttu-id="85d55-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="85d55-134">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="85d55-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="85d55-135">Authorization</span></span>  | <span data-ttu-id="85d55-136">string</span><span class="sxs-lookup"><span data-stu-id="85d55-136">string</span></span> | <span data-ttu-id="85d55-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85d55-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="85d55-139">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="85d55-139">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="85d55-140">string</span><span class="sxs-lookup"><span data-stu-id="85d55-140">string</span></span> | <span data-ttu-id="85d55-141">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="85d55-141">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="85d55-142">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="85d55-142">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="85d55-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="85d55-143">Optional.</span></span> |
| <span data-ttu-id="85d55-144">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="85d55-144">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="85d55-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85d55-145">string</span></span> | <span data-ttu-id="85d55-146">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="85d55-146">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="85d55-147">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="85d55-147">Values can be "text" or "html".</span></span> <span data-ttu-id="85d55-148">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="85d55-148">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="85d55-149">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="85d55-149">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="85d55-150">Opcional.</span><span class="sxs-lookup"><span data-stu-id="85d55-150">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85d55-151">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85d55-151">Request body</span></span>
<span data-ttu-id="85d55-152">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85d55-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85d55-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="85d55-153">Response</span></span>
<span data-ttu-id="85d55-154">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85d55-154">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85d55-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85d55-155">Example</span></span>
#### <a name="request"></a><span data-ttu-id="85d55-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85d55-156">Request</span></span>
<span data-ttu-id="85d55-157">O exemplo a seguir solicita que corpos de evento sejam retornados no formato de texto.</span><span class="sxs-lookup"><span data-stu-id="85d55-157">The following example requests event bodies to be returned in text format.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarviews"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-10-01T19:00:00.00
Prefer: outlook.body-content-type="text"
```

#### <a name="response"></a><span data-ttu-id="85d55-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="85d55-158">Response</span></span>
<span data-ttu-id="85d55-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="85d55-159">The following is an example of the response.</span></span>
><span data-ttu-id="85d55-160">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="85d55-160">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="85d55-161">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85d55-161">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1354
Preference-Applied: outlook.body-content-type="text"

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('02bd9fd6-8f93-4758-87c3-1fb73740a315')/calendarView",
    "@odata.nextLink":"https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19%3a00%3a00.0000000&endDateTime=2017-10-01T19%3a00%3a00.00&$skip=10",
    "value":[
        {
            "@odata.etag":"W/\"xPZF2y46pEiVBni87OnrpgAAFq78Xw==\"",
            "id":"AAMkAGI5MWYJOwAAEA==",
            "createdDateTime":"2017-07-31T18:59:01.982289Z",
            "lastModifiedDateTime":"2017-09-06T04:29:38.6647687Z",
            "changeKey":"xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
            "categories":[

            ],
            "originalStartTimeZone":"Eastern Standard Time",
            "originalEndTimeZone":"Eastern Standard Time",
            "uid":"040000008200E00074C5B7101A82E00807E1080E824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
            "reminderMinutesBeforeStart":15,
            "isReminderOn":true,
            "hasAttachments":false,
            "subject":"New Training Plans",
            "bodyPreview":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
            "importance":"normal",
            "sensitivity":"normal",
            "isAllDay":false,
            "isCancelled":false,
            "isOrganizer":true,
            "responseRequested":true,
            "seriesMasterId":null,
            "showAs":"busy",
            "type":"singleInstance",
            "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI5MWYJOwAAEA%3D%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl":null,
            "responseStatus":{
                "response":"organizer",
                "time":"0001-01-01T00:00:00Z"
            },
            "body":{
                "contentType":"text",
                "content":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>\r\n"
            },
            "start":{
                "dateTime":"2017-08-14T21:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2017-08-14T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"HR Taskforce / Facilities"
            },
            "recurrence":null,
            "attendees":[
                 {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"HR Taskforce",
                        "address":"HRTaskforce@contoso.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Megan Bowen",
                        "address":"MeganB@contoso.onmicrosoft.com"
                    }
                }
             ],
            "organizer":{
                "emailAddress":{
                    "name":"HR Taskforce",
                    "address":"HRTaskforce@contoso.onmicrosoft.com"
                }
            }
        },
        {
            "@odata.etag":"W/\"xPZF2y46pEiVBni87OnrpgAAFq78Xw==\"",
            "id":"AAMkAGI5MWYJOwAAEA==",
            "createdDateTime":"2017-07-31T18:59:01.982289Z",
            "lastModifiedDateTime":"2017-09-06T04:29:38.6647687Z",
            "changeKey":"xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
            "categories":[

            ],
            "originalStartTimeZone":"Eastern Standard Time",
            "originalEndTimeZone":"Eastern Standard Time",
            "uid":"040000008200E00074C5B7101A82E00807E10810824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
            "reminderMinutesBeforeStart":15,
            "isReminderOn":true,
            "hasAttachments":false,
            "subject":"New Training Plans",
            "bodyPreview":"Follow-up meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
            "importance":"normal",
            "sensitivity":"normal",
            "isAllDay":false,
            "isCancelled":false,
            "isOrganizer":true,
            "responseRequested":true,
            "seriesMasterId":null,
            "showAs":"busy",
            "type":"singleInstance",
            "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI5MWYJOwAAEA%3D%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl":null,
            "responseStatus":{
                "response":"organizer",
                "time":"0001-01-01T00:00:00Z"
            },
            "body":{
                "contentType":"text",
                "content":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>\r\n"
            },
            "start":{
                "dateTime":"2017-08-16T21:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2017-08-16T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"HR Taskforce / Facilities"
            },
            "recurrence":null,
            "attendees":[
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"HR Taskforce",
                        "address":"HRTaskforce@contoso.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Megan Bowen",
                        "address":"MeganB@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer":{
                "emailAddress":{
                    "name":"HR Taskforce",
                    "address":"HRTaskforce@contoso.onmicrosoft.com"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
