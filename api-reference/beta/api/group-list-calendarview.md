---
title: Listar calendarView
description: Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida, do calendário padrão de um grupo.
ms.openlocfilehash: 25090591750ed556407159f3744113b08d25fcae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036184"
---
# <a name="list-calendarview"></a><span data-ttu-id="3a739-103">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="3a739-103">List calendarView</span></span>

> <span data-ttu-id="3a739-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3a739-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a739-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3a739-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a739-106">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida, do calendário padrão de um grupo.</span><span class="sxs-lookup"><span data-stu-id="3a739-106">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a739-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a739-107">Permissions</span></span>
<span data-ttu-id="3a739-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a739-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a739-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a739-110">Permission type</span></span>      | <span data-ttu-id="3a739-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a739-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a739-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a739-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3a739-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a739-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3a739-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a739-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a739-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a739-115">Not supported.</span></span>    |
|<span data-ttu-id="3a739-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a739-116">Application</span></span> | <span data-ttu-id="3a739-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a739-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a739-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a739-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="3a739-119">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="3a739-119">Query parameters</span></span>
<span data-ttu-id="3a739-120">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="3a739-120">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="3a739-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3a739-121">Parameter</span></span>    | <span data-ttu-id="3a739-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a739-122">Type</span></span>   |<span data-ttu-id="3a739-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a739-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a739-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3a739-124">startDateTime</span></span>|<span data-ttu-id="3a739-125">String</span><span class="sxs-lookup"><span data-stu-id="3a739-125">String</span></span>|<span data-ttu-id="3a739-p103">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="3a739-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="3a739-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3a739-128">endDateTime</span></span>|<span data-ttu-id="3a739-129">String</span><span class="sxs-lookup"><span data-stu-id="3a739-129">String</span></span>|<span data-ttu-id="3a739-p104">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="3a739-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="3a739-132">Este método também dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3a739-132">This method also supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a739-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a739-133">Request headers</span></span>
| <span data-ttu-id="3a739-134">Nome</span><span class="sxs-lookup"><span data-stu-id="3a739-134">Name</span></span>       | <span data-ttu-id="3a739-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a739-135">Type</span></span> | <span data-ttu-id="3a739-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a739-136">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="3a739-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a739-137">Authorization</span></span>  | <span data-ttu-id="3a739-138">string</span><span class="sxs-lookup"><span data-stu-id="3a739-138">string</span></span> | <span data-ttu-id="3a739-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a739-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3a739-141">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="3a739-141">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="3a739-142">string</span><span class="sxs-lookup"><span data-stu-id="3a739-142">string</span></span> | <span data-ttu-id="3a739-143">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="3a739-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="3a739-144">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="3a739-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="3a739-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3a739-145">Optional.</span></span> |
| <span data-ttu-id="3a739-146">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="3a739-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="3a739-147">string</span><span class="sxs-lookup"><span data-stu-id="3a739-147">string</span></span> | <span data-ttu-id="3a739-148">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="3a739-148">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="3a739-149">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="3a739-149">Values can be "text" or "html".</span></span> <span data-ttu-id="3a739-150">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="3a739-150">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="3a739-151">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="3a739-151">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="3a739-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3a739-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a739-153">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a739-153">Request body</span></span>
<span data-ttu-id="3a739-154">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a739-154">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a739-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a739-155">Response</span></span>
<span data-ttu-id="3a739-156">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a739-156">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a739-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a739-157">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3a739-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a739-158">Request</span></span>
<span data-ttu-id="3a739-159">O exemplo a seguir solicita que corpos de evento sejam retornados no formato de texto.</span><span class="sxs-lookup"><span data-stu-id="3a739-159">The following example requests event bodies to be returned in text format.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarviews"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-10-01T19:00:00.00
Prefer: outlook.body-content-type="text"
```

#### <a name="response"></a><span data-ttu-id="3a739-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a739-160">Response</span></span>
<span data-ttu-id="3a739-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3a739-161">The following is an example of the response.</span></span>
><span data-ttu-id="3a739-162">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3a739-162">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3a739-163">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a739-163">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
