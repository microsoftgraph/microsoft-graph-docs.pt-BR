---
title: Listar eventos
description: Recuperar uma lista de objetos event.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 908a80a1b4d021add8056257bb0a304b3b8d8a55
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441720"
---
# <a name="list-events"></a><span data-ttu-id="2325d-103">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="2325d-103">List events</span></span>
<span data-ttu-id="2325d-104">Recupere uma lista de objetos [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="2325d-104">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2325d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2325d-105">Permissions</span></span>
<span data-ttu-id="2325d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2325d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2325d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2325d-108">Permission type</span></span>      | <span data-ttu-id="2325d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2325d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2325d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2325d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2325d-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2325d-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2325d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2325d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2325d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2325d-113">Not supported.</span></span>    |
|<span data-ttu-id="2325d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2325d-114">Application</span></span> | <span data-ttu-id="2325d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2325d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2325d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2325d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2325d-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2325d-117">Optional query parameters</span></span>
<span data-ttu-id="2325d-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2325d-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2325d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2325d-119">Request headers</span></span>
| <span data-ttu-id="2325d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2325d-120">Name</span></span>       | <span data-ttu-id="2325d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2325d-121">Type</span></span> | <span data-ttu-id="2325d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2325d-122">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="2325d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2325d-123">Authorization</span></span>  | <span data-ttu-id="2325d-124">string</span><span class="sxs-lookup"><span data-stu-id="2325d-124">string</span></span> | <span data-ttu-id="2325d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2325d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2325d-127">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="2325d-127">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="2325d-128">string</span><span class="sxs-lookup"><span data-stu-id="2325d-128">string</span></span> | <span data-ttu-id="2325d-129">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="2325d-129">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="2325d-130">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="2325d-130">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="2325d-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2325d-131">Optional.</span></span> |
| <span data-ttu-id="2325d-132">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="2325d-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="2325d-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2325d-133">string</span></span> | <span data-ttu-id="2325d-134">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="2325d-134">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="2325d-135">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="2325d-135">Values can be "text" or "html".</span></span> <span data-ttu-id="2325d-136">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="2325d-136">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="2325d-137">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="2325d-137">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="2325d-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2325d-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2325d-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2325d-139">Request body</span></span>
<span data-ttu-id="2325d-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2325d-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2325d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2325d-141">Response</span></span>
<span data-ttu-id="2325d-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2325d-142">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2325d-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2325d-143">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2325d-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2325d-144">Request</span></span>
<span data-ttu-id="2325d-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2325d-145">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2325d-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="2325d-146">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315"],
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2325d-147">C#</span><span class="sxs-lookup"><span data-stu-id="2325d-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2325d-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="2325d-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2325d-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2325d-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2325d-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="2325d-150">Response</span></span>
<span data-ttu-id="2325d-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2325d-151">The following is an example of the response.</span></span>
><span data-ttu-id="2325d-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2325d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA==",
      "createdDateTime": "2017-07-31T18:59:01.982289Z",
      "lastModifiedDateTime": "2017-09-06T04:29:38.6647687Z",
      "changeKey": "xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
      "categories": [],
      "originalStartTimeZone": "Eastern Standard Time",
      "originalEndTimeZone": "Eastern Standard Time",
      "iCalUId": "040000008200E00074C5B7101A82E00800000000824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
      "reminderMinutesBeforeStart": 15,
      "isReminderOn": true,
      "hasAttachments": false,
      "subject": "New Training Plans",
      "bodyPreview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
      "importance": "normal",
      "sensitivity": "normal",
      "isAllDay": false,
      "isCancelled": false,
      "isOrganizer": true,
      "responseRequested": true,
      "seriesMasterId": null,
      "showAs": "busy",
      "type": "seriesMaster",
      "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA%3D%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl": null,
      "responseStatus": {
          "response": "organizer",
          "time": "0001-01-01T00:00:00Z"
      },
      "body": {
          "contentType": "html",
          "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Meeting to plan new trainings.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
      },
      "start": {
          "dateTime": "2017-08-14T21:00:00.0000000",
          "timeZone": "UTC"
      },
      "end": {
          "dateTime": "2017-08-14T22:00:00.0000000",
          "timeZone": "UTC"
      },
      "location": {
          "displayName": "HR Taskforce / Facilities"
      },
      "recurrence": {
          "pattern": {
              "type": "weekly",
              "interval": 1,
              "month": 0,
              "dayOfMonth": 0,
              "daysOfWeek": [
                  "monday",
                  "wednesday",
                  "friday"
              ],
              "firstDayOfWeek": "sunday",
              "index": "first"
          },
          "range": {
              "type": "noEnd",
              "startDate": "2017-08-14",
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
                  "time": "2017-07-31T18:59:06.4180028Z"
              },
              "emailAddress": {
                  "name": "Joni Sherman",
                  "address": "JoniS@contoso.onmicrosoft.com"
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
                  "address": "HRTaskforce@contoso.onmicrosoft.com"
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
                  "address": "MeganB@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Lidia Holloway",
                  "address": "LidiaH@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Emily Braun",
                  "address": "EmilyB@contoso.onmicrosoft.com"
              }
          }
      ],
      "organizer": {
          "emailAddress": {
              "name": "HR Taskforce",
              "address": "HRTaskforce@contoso.onmicrosoft.com"
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
