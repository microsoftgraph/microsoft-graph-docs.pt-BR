---
title: 'calendar: getSchedule'
description: Obtenha as informações de disponibilidade para um conjunto de usuários, listas de distribuição ou recursos para um período especificado.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 48283f7e81a1faea34d91dec72906b71361c816a
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869376"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="7e361-103">calendar: getSchedule</span><span class="sxs-lookup"><span data-stu-id="7e361-103">calendar: getSchedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e361-104">Adquira as informações de disponibilidade para um conjunto de usuários, listas de distribuição ou recursos (salas e equipamentos) para um período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="7e361-104">Get the free/busy availability information for a collection of users, distributions lists, or resources, for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e361-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e361-105">Permissions</span></span>
<span data-ttu-id="7e361-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e361-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e361-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e361-108">Permission type</span></span>      | <span data-ttu-id="7e361-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e361-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e361-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e361-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7e361-111">Calendar.Read, Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e361-111">Calendar.Read, Calendar.ReadWrite</span></span>    |
|<span data-ttu-id="7e361-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e361-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e361-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e361-113">Not supported.</span></span> |
|<span data-ttu-id="7e361-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e361-114">Application</span></span> | <span data-ttu-id="7e361-115">Calendar.Read, Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e361-115">Calendar.Read, Calendar.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e361-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e361-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="7e361-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e361-117">Request headers</span></span>
| <span data-ttu-id="7e361-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7e361-118">Name</span></span>       | <span data-ttu-id="7e361-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e361-119">Type</span></span> | <span data-ttu-id="7e361-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e361-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7e361-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e361-121">Authorization</span></span>  | <span data-ttu-id="7e361-122">string</span><span class="sxs-lookup"><span data-stu-id="7e361-122">string</span></span>  | <span data-ttu-id="7e361-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e361-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e361-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e361-125">Content-Type</span></span>  | <span data-ttu-id="7e361-126">string</span><span class="sxs-lookup"><span data-stu-id="7e361-126">string</span></span> | <span data-ttu-id="7e361-127">Natureza dos dados no corpo de uma entidade, que é application/json.</span><span class="sxs-lookup"><span data-stu-id="7e361-127">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="7e361-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e361-128">Required.</span></span>  |
| <span data-ttu-id="7e361-129">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="7e361-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="7e361-130">string</span><span class="sxs-lookup"><span data-stu-id="7e361-130">string</span></span> | <span data-ttu-id="7e361-131">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="7e361-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="7e361-132">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="7e361-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="7e361-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7e361-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e361-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e361-134">Request body</span></span>
<span data-ttu-id="7e361-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e361-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7e361-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e361-136">Property</span></span>     | <span data-ttu-id="7e361-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e361-137">Type</span></span>   |<span data-ttu-id="7e361-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e361-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e361-139">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="7e361-139">availabilityViewInterval</span></span>|<span data-ttu-id="7e361-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7e361-140">Int32</span></span>|<span data-ttu-id="7e361-141">Representa a duração de um intervalo de tempo em \*\* availabilityView \*\* na resposta.</span><span class="sxs-lookup"><span data-stu-id="7e361-141">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="7e361-142">O padrão é 30 minutos, o mínimo é 6, o máximo é 1440.</span><span class="sxs-lookup"><span data-stu-id="7e361-142">The default is 30 minutes, minimum is 6, maximum is 1440.</span></span> <span data-ttu-id="7e361-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7e361-143">Optional.</span></span>|
|<span data-ttu-id="7e361-144">endTime</span><span class="sxs-lookup"><span data-stu-id="7e361-144">endTime</span></span>|[<span data-ttu-id="7e361-145">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="7e361-145">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="7e361-146">A data, a hora e o fuso horário em que o período termina.</span><span class="sxs-lookup"><span data-stu-id="7e361-146">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="7e361-147">agendas</span><span class="sxs-lookup"><span data-stu-id="7e361-147">schedules</span></span>|<span data-ttu-id="7e361-148">Coleção String</span><span class="sxs-lookup"><span data-stu-id="7e361-148">String collection</span></span>|<span data-ttu-id="7e361-149">Uma coleção de endereços SMTP de usuários, listas de distribuição ou recursos para obter informações sobre disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="7e361-149">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="7e361-150">startTime</span><span class="sxs-lookup"><span data-stu-id="7e361-150">startTime</span></span>|[<span data-ttu-id="7e361-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="7e361-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="7e361-152">A data, a hora e o fuso horário em que o período começa.</span><span class="sxs-lookup"><span data-stu-id="7e361-152">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="7e361-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e361-153">Response</span></span>

<span data-ttu-id="7e361-154">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [scheduleInformation](../resources/scheduleinformation.md) para cada objeto no parâmetro `schedules`.</span><span class="sxs-lookup"><span data-stu-id="7e361-154">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="7e361-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e361-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e361-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e361-156">Request</span></span>
<span data-ttu-id="7e361-157">O exemplo a seguir obtém as informações de disponibilidade de dois usuários em relação à data, a hora e o fuso horário especificados.</span><span class="sxs-lookup"><span data-stu-id="7e361-157">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/getschedule 
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

##### <a name="response"></a><span data-ttu-id="7e361-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e361-158">Response</span></span>
<span data-ttu-id="7e361-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e361-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.scheduleInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.scheduleInformation)",
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
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/calendar-getschedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
