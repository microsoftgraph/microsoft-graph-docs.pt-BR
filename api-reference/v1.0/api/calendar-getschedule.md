---
title: 'calendar: getSchedule'
description: Obtenha as informações de disponibilidade para um conjunto de usuários, listas de distribuição ou recursos para um período especificado.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: de04a0771b5d4d298140fa150ba414a47bc3d094
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023378"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="93d07-103">calendar: getSchedule</span><span class="sxs-lookup"><span data-stu-id="93d07-103">calendar: getSchedule</span></span>

<span data-ttu-id="93d07-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93d07-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93d07-105">Adquira as informações de disponibilidade para um conjunto de usuários, listas de distribuição ou recursos (salas e equipamentos) para um período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="93d07-105">Get the free/busy availability information for a collection of users, distributions lists, or resources (rooms or equipment) for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="93d07-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="93d07-106">Permissions</span></span>
<span data-ttu-id="93d07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93d07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93d07-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93d07-109">Permission type</span></span>      | <span data-ttu-id="93d07-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93d07-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93d07-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93d07-111">Delegated (work or school account)</span></span> | <span data-ttu-id="93d07-112">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93d07-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="93d07-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93d07-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93d07-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93d07-114">Not supported.</span></span> |
|<span data-ttu-id="93d07-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93d07-115">Application</span></span> | <span data-ttu-id="93d07-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93d07-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="93d07-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93d07-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="93d07-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93d07-118">Request headers</span></span>
| <span data-ttu-id="93d07-119">Nome</span><span class="sxs-lookup"><span data-stu-id="93d07-119">Name</span></span>       | <span data-ttu-id="93d07-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="93d07-120">Type</span></span> | <span data-ttu-id="93d07-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="93d07-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="93d07-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="93d07-122">Authorization</span></span>  | <span data-ttu-id="93d07-123">string</span><span class="sxs-lookup"><span data-stu-id="93d07-123">string</span></span>  | <span data-ttu-id="93d07-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93d07-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93d07-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="93d07-126">Content-Type</span></span>  | <span data-ttu-id="93d07-127">string</span><span class="sxs-lookup"><span data-stu-id="93d07-127">string</span></span> | <span data-ttu-id="93d07-128">Natureza dos dados no corpo de uma entidade, que é application/json.</span><span class="sxs-lookup"><span data-stu-id="93d07-128">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="93d07-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93d07-129">Required.</span></span>  |
| <span data-ttu-id="93d07-130">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="93d07-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="93d07-131">string</span><span class="sxs-lookup"><span data-stu-id="93d07-131">string</span></span> | <span data-ttu-id="93d07-132">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="93d07-132">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="93d07-133">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="93d07-133">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="93d07-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="93d07-134">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93d07-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93d07-135">Request body</span></span>
<span data-ttu-id="93d07-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93d07-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="93d07-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93d07-137">Property</span></span>     | <span data-ttu-id="93d07-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="93d07-138">Type</span></span>   |<span data-ttu-id="93d07-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="93d07-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93d07-140">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="93d07-140">availabilityViewInterval</span></span>|<span data-ttu-id="93d07-141">Int32</span><span class="sxs-lookup"><span data-stu-id="93d07-141">Int32</span></span>|<span data-ttu-id="93d07-142">Representa a duração de um intervalo de tempo em \*\* availabilityView \*\* na resposta.</span><span class="sxs-lookup"><span data-stu-id="93d07-142">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="93d07-143">O padrão é 30 minutos, o mínimo é 5, o máximo é 1440.</span><span class="sxs-lookup"><span data-stu-id="93d07-143">The default is 30 minutes, minimum is 5, maximum is 1440.</span></span> <span data-ttu-id="93d07-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="93d07-144">Optional.</span></span>|
|<span data-ttu-id="93d07-145">endTime</span><span class="sxs-lookup"><span data-stu-id="93d07-145">endTime</span></span>|[<span data-ttu-id="93d07-146">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="93d07-146">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="93d07-147">A data, a hora e o fuso horário em que o período termina.</span><span class="sxs-lookup"><span data-stu-id="93d07-147">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="93d07-148">agendas</span><span class="sxs-lookup"><span data-stu-id="93d07-148">schedules</span></span>|<span data-ttu-id="93d07-149">Coleção String</span><span class="sxs-lookup"><span data-stu-id="93d07-149">String collection</span></span>|<span data-ttu-id="93d07-150">Uma coleção de endereços SMTP de usuários, listas de distribuição ou recursos para obter informações sobre disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="93d07-150">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="93d07-151">startTime</span><span class="sxs-lookup"><span data-stu-id="93d07-151">startTime</span></span>|[<span data-ttu-id="93d07-152">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="93d07-152">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="93d07-153">A data, a hora e o fuso horário em que o período começa.</span><span class="sxs-lookup"><span data-stu-id="93d07-153">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="93d07-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="93d07-154">Response</span></span>

<span data-ttu-id="93d07-155">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [scheduleInformation](../resources/scheduleinformation.md) para cada objeto no parâmetro `schedules`.</span><span class="sxs-lookup"><span data-stu-id="93d07-155">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="93d07-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93d07-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93d07-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93d07-157">Request</span></span>
<span data-ttu-id="93d07-158">O exemplo a seguir obtém as informações de disponibilidade de dois usuários em relação à data, a hora e o fuso horário especificados.</span><span class="sxs-lookup"><span data-stu-id="93d07-158">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>


# <a name="http"></a>[<span data-ttu-id="93d07-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="93d07-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="93d07-160">C#</span><span class="sxs-lookup"><span data-stu-id="93d07-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-getschedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93d07-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93d07-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-getschedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93d07-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93d07-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-getschedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93d07-163">Java</span><span class="sxs-lookup"><span data-stu-id="93d07-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendar-getschedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="93d07-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="93d07-164">Response</span></span>
<span data-ttu-id="93d07-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93d07-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

