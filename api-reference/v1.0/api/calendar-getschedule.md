---
title: 'calendar: getSchedule'
description: Obtenha as informações de disponibilidade para um conjunto de usuários, listas de distribuição ou recursos para um período especificado.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d604c6554f88e556c37a9ad3c89c61a43b63326c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325320"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="1f538-103">calendar: getSchedule</span><span class="sxs-lookup"><span data-stu-id="1f538-103">calendar: getSchedule</span></span>

<span data-ttu-id="1f538-104">Adquira as informações de disponibilidade para um conjunto de usuários, listas de distribuição ou recursos (salas e equipamentos) para um período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="1f538-104">Get the free/busy availability information for a collection of users, distributions lists, or resources (rooms or equipment) for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f538-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f538-105">Permissions</span></span>
<span data-ttu-id="1f538-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f538-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f538-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f538-108">Permission type</span></span>      | <span data-ttu-id="1f538-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f538-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f538-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f538-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1f538-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f538-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1f538-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f538-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f538-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f538-113">Not supported.</span></span> |
|<span data-ttu-id="1f538-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f538-114">Application</span></span> | <span data-ttu-id="1f538-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f538-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f538-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f538-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="1f538-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f538-117">Request headers</span></span>
| <span data-ttu-id="1f538-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1f538-118">Name</span></span>       | <span data-ttu-id="1f538-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f538-119">Type</span></span> | <span data-ttu-id="1f538-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f538-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1f538-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f538-121">Authorization</span></span>  | <span data-ttu-id="1f538-122">string</span><span class="sxs-lookup"><span data-stu-id="1f538-122">string</span></span>  | <span data-ttu-id="1f538-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f538-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f538-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f538-125">Content-Type</span></span>  | <span data-ttu-id="1f538-126">string</span><span class="sxs-lookup"><span data-stu-id="1f538-126">string</span></span> | <span data-ttu-id="1f538-127">Natureza dos dados no corpo de uma entidade, que é application/json.</span><span class="sxs-lookup"><span data-stu-id="1f538-127">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="1f538-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f538-128">Required.</span></span>  |
| <span data-ttu-id="1f538-129">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="1f538-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="1f538-130">string</span><span class="sxs-lookup"><span data-stu-id="1f538-130">string</span></span> | <span data-ttu-id="1f538-131">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="1f538-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="1f538-132">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="1f538-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="1f538-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1f538-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f538-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f538-134">Request body</span></span>
<span data-ttu-id="1f538-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f538-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1f538-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f538-136">Property</span></span>     | <span data-ttu-id="1f538-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f538-137">Type</span></span>   |<span data-ttu-id="1f538-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f538-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f538-139">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="1f538-139">availabilityViewInterval</span></span>|<span data-ttu-id="1f538-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1f538-140">Int32</span></span>|<span data-ttu-id="1f538-141">Representa a duração de um intervalo de tempo em \*\* availabilityView \*\* na resposta.</span><span class="sxs-lookup"><span data-stu-id="1f538-141">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="1f538-142">O padrão é 30 minutos, o mínimo é 6, o máximo é 1440.</span><span class="sxs-lookup"><span data-stu-id="1f538-142">The default is 30 minutes, minimum is 6, maximum is 1440.</span></span> <span data-ttu-id="1f538-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1f538-143">Optional.</span></span>|
|<span data-ttu-id="1f538-144">endTime</span><span class="sxs-lookup"><span data-stu-id="1f538-144">endTime</span></span>|[<span data-ttu-id="1f538-145">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="1f538-145">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="1f538-146">A data, a hora e o fuso horário em que o período termina.</span><span class="sxs-lookup"><span data-stu-id="1f538-146">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="1f538-147">agendas</span><span class="sxs-lookup"><span data-stu-id="1f538-147">schedules</span></span>|<span data-ttu-id="1f538-148">Coleção String</span><span class="sxs-lookup"><span data-stu-id="1f538-148">String collection</span></span>|<span data-ttu-id="1f538-149">Uma coleção de endereços SMTP de usuários, listas de distribuição ou recursos para obter informações sobre disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="1f538-149">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="1f538-150">startTime</span><span class="sxs-lookup"><span data-stu-id="1f538-150">startTime</span></span>|[<span data-ttu-id="1f538-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="1f538-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="1f538-152">A data, a hora e o fuso horário em que o período começa.</span><span class="sxs-lookup"><span data-stu-id="1f538-152">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="1f538-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f538-153">Response</span></span>

<span data-ttu-id="1f538-154">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [scheduleInformation](../resources/scheduleinformation.md) para cada objeto no parâmetro `schedules`.</span><span class="sxs-lookup"><span data-stu-id="1f538-154">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="1f538-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f538-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f538-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f538-156">Request</span></span>
<span data-ttu-id="1f538-157">O exemplo a seguir obtém as informações de disponibilidade de dois usuários em relação à data, a hora e o fuso horário especificados.</span><span class="sxs-lookup"><span data-stu-id="1f538-157">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1f538-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f538-158">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_getSchedule"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendar/getschedule 
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{        
    "schedules": ["adelev@contoso.onmicrosoft.com", "meganb@contoso.onmicrosoft.com"],
    "startTime": {
        "dateTime": "2019-03-15T09:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "endTime": {
        "dateTime": "2019-03-15T18:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "availabilityViewInterval": "60"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1f538-159">C#</span><span class="sxs-lookup"><span data-stu-id="1f538-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-getschedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1f538-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f538-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-getschedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1f538-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f538-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-getschedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1f538-162">Java</span><span class="sxs-lookup"><span data-stu-id="1f538-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendar-getschedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1f538-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f538-163">Response</span></span>
<span data-ttu-id="1f538-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f538-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scheduleInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value": [
        {
            "scheduleId": "adelev@contoso.onmicrosoft.com",
            "availabilityView": "000220000",
            "scheduleItems": [
                {
                    "isPrivate": false,
                    "status": "busy",
                    "subject": "Let's go for lunch",
                    "location": "Harry's Bar",
                    "start": {
                        "dateTime": "2019-03-15T12:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T14:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                }
            ],
            "workingHours": {
                "daysOfWeek": [
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime": "08:00:00.0000000",
                "endTime": "17:00:00.0000000",
                "timeZone": {
                    "name": "Pacific Standard Time"
                }
            }
        },
        {
            "scheduleId": "meganb@contoso.onmicrosoft.com",
            "availabilityView": "200220010",
            "scheduleItems": [
                {
                    "status": "busy",
                    "start": {
                        "dateTime": "2019-03-15T08:30:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T09:30:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                {
                    "status": "busy",
                    "start": {
                        "dateTime": "2019-03-15T12:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T14:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                {
                    "status": "tentative",
                    "start": {
                        "dateTime": "2019-03-15T12:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T13:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                {
                    "status": "busy",
                    "start": {
                        "dateTime": "2019-03-15T13:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T14:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                {
                    "status": "tentative",
                    "start": {
                        "dateTime": "2019-03-15T16:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T17:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                }
            ],
            "workingHours": {
                "daysOfWeek": [
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime": "08:00:00.0000000",
                "endTime": "17:00:00.0000000",
                "timeZone": {
                    "@odata.type": "#microsoft.graph.customTimeZone",
                    "bias": 480,
                    "name": "Customized Time Zone",
                    "standardOffset": {
                        "time": "02:00:00.0000000",
                        "dayOccurrence": 1,
                        "dayOfWeek": "sunday",
                        "month": 11,
                        "year": 0
                    },
                    "daylightOffset": {
                        "daylightBias": -60,
                        "time": "02:00:00.0000000",
                        "dayOccurrence": 2,
                        "dayOfWeek": "sunday",
                        "month": 3,
                        "year": 0
                    }
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
  "description": "calendar: getSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
