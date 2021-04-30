---
title: 'calendar: getSchedule'
description: Obtenha as informações de disponibilidade para um conjunto de usuários, listas de distribuição ou recursos para um período especificado.
localization_priority: Priority
author: tariq-sharif
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 267da79cf32f55de94b6d23fd87125c415973f03
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054606"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="dddc3-103">calendar: getSchedule</span><span class="sxs-lookup"><span data-stu-id="dddc3-103">calendar: getSchedule</span></span>

<span data-ttu-id="dddc3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dddc3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dddc3-105">Adquira as informações de disponibilidade para um conjunto de usuários, listas de distribuição ou recursos (salas e equipamentos) para um período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="dddc3-105">Get the free/busy availability information for a collection of users, distributions lists, or resources (rooms or equipment) for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="dddc3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dddc3-106">Permissions</span></span>
<span data-ttu-id="dddc3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dddc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dddc3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dddc3-109">Permission type</span></span>      | <span data-ttu-id="dddc3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dddc3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dddc3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dddc3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dddc3-112">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dddc3-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="dddc3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dddc3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dddc3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dddc3-114">Not supported.</span></span> |
|<span data-ttu-id="dddc3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dddc3-115">Application</span></span> | <span data-ttu-id="dddc3-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dddc3-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dddc3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dddc3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="dddc3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dddc3-118">Request headers</span></span>
| <span data-ttu-id="dddc3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dddc3-119">Name</span></span>       | <span data-ttu-id="dddc3-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="dddc3-120">Type</span></span> | <span data-ttu-id="dddc3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dddc3-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dddc3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dddc3-122">Authorization</span></span>  | <span data-ttu-id="dddc3-123">string</span><span class="sxs-lookup"><span data-stu-id="dddc3-123">string</span></span>  | <span data-ttu-id="dddc3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dddc3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dddc3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dddc3-126">Content-Type</span></span>  | <span data-ttu-id="dddc3-127">string</span><span class="sxs-lookup"><span data-stu-id="dddc3-127">string</span></span> | <span data-ttu-id="dddc3-p103">Natureza dos dados no corpo de uma entidade, que é application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dddc3-p103">Nature of the data in the body of an entity, which is application/json. Required.</span></span>  |
| <span data-ttu-id="dddc3-130">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="dddc3-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="dddc3-131">string</span><span class="sxs-lookup"><span data-stu-id="dddc3-131">string</span></span> | <span data-ttu-id="dddc3-p104">Use isso para especificar o fuso horário para os horários de início e término na resposta. Se não for especificado, esses valores de tempo serão retornados em UTC. Opcional.</span><span class="sxs-lookup"><span data-stu-id="dddc3-p104">Use this to specify the time zone for start and end times in the response. If not specified, those time values are returned in UTC. Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dddc3-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dddc3-135">Request body</span></span>
<span data-ttu-id="dddc3-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dddc3-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dddc3-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dddc3-137">Property</span></span>     | <span data-ttu-id="dddc3-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="dddc3-138">Type</span></span>   |<span data-ttu-id="dddc3-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="dddc3-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dddc3-140">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="dddc3-140">availabilityViewInterval</span></span>|<span data-ttu-id="dddc3-141">Int32</span><span class="sxs-lookup"><span data-stu-id="dddc3-141">Int32</span></span>|<span data-ttu-id="dddc3-142">Representa a duração de um intervalo de tempo em **availabilityView** na resposta.</span><span class="sxs-lookup"><span data-stu-id="dddc3-142">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="dddc3-143">O padrão é 30 minutos, o mínimo é 5, o máximo é 1440.</span><span class="sxs-lookup"><span data-stu-id="dddc3-143">The default is 30 minutes, minimum is 5, maximum is 1440.</span></span> <span data-ttu-id="dddc3-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dddc3-144">Optional.</span></span>|
|<span data-ttu-id="dddc3-145">endTime</span><span class="sxs-lookup"><span data-stu-id="dddc3-145">endTime</span></span>|[<span data-ttu-id="dddc3-146">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="dddc3-146">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="dddc3-147">A data, a hora e o fuso horário em que o período termina.</span><span class="sxs-lookup"><span data-stu-id="dddc3-147">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="dddc3-148">agendas</span><span class="sxs-lookup"><span data-stu-id="dddc3-148">schedules</span></span>|<span data-ttu-id="dddc3-149">Coleção String</span><span class="sxs-lookup"><span data-stu-id="dddc3-149">String collection</span></span>|<span data-ttu-id="dddc3-150">Uma coleção de endereços SMTP de usuários, listas de distribuição ou recursos para obter informações sobre disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="dddc3-150">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="dddc3-151">startTime</span><span class="sxs-lookup"><span data-stu-id="dddc3-151">startTime</span></span>|[<span data-ttu-id="dddc3-152">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="dddc3-152">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="dddc3-153">A data, a hora e o fuso horário em que o período começa.</span><span class="sxs-lookup"><span data-stu-id="dddc3-153">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="dddc3-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="dddc3-154">Response</span></span>

<span data-ttu-id="dddc3-155">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [scheduleInformation](../resources/scheduleinformation.md) para cada objeto no parâmetro `schedules`.</span><span class="sxs-lookup"><span data-stu-id="dddc3-155">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="dddc3-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dddc3-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dddc3-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dddc3-157">Request</span></span>
<span data-ttu-id="dddc3-158">O exemplo a seguir obtém as informações de disponibilidade de dois usuários em relação à data, a hora e o fuso horário especificados.</span><span class="sxs-lookup"><span data-stu-id="dddc3-158">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>


# <a name="http"></a>[<span data-ttu-id="dddc3-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="dddc3-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_getSchedule"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendar/getSchedule 
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
    "availabilityViewInterval": 60
}
```
# <a name="c"></a>[<span data-ttu-id="dddc3-160">C#</span><span class="sxs-lookup"><span data-stu-id="dddc3-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-getschedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dddc3-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dddc3-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-getschedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dddc3-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dddc3-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-getschedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dddc3-163">Java</span><span class="sxs-lookup"><span data-stu-id="dddc3-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendar-getschedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dddc3-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="dddc3-164">Response</span></span>
<span data-ttu-id="dddc3-165">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dddc3-165">Here is an example of the response.</span></span> <span data-ttu-id="dddc3-166">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dddc3-166">Note: The response object shown here might be shortened for readability.</span></span>
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

