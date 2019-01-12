---
title: 'calendário: getSchedule'
description: Obtenha as informações de disponibilidade para um conjunto de usuários, recursos ou listas de Distribuições por um período de tempo especificado.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 9089489d2b26b3dd4cd56b950538a72ab533c933
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956952"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="610a0-103">calendário: getSchedule</span><span class="sxs-lookup"><span data-stu-id="610a0-103">calendar: getSchedule</span></span>

> <span data-ttu-id="610a0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="610a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="610a0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="610a0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="610a0-106">Obtenha as informações de disponibilidade para um conjunto de usuários, recursos ou listas de Distribuições por um período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="610a0-106">Get the free/busy availability information for a collection of users, distributions lists, or resources, for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="610a0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="610a0-107">Permissions</span></span>
<span data-ttu-id="610a0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="610a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="610a0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="610a0-110">Permission type</span></span>      | <span data-ttu-id="610a0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="610a0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="610a0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="610a0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="610a0-113">Calendar.Read, Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="610a0-113">Calendar.Read, Calendar.ReadWrite</span></span>    |
|<span data-ttu-id="610a0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="610a0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="610a0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="610a0-115">Not supported.</span></span> |
|<span data-ttu-id="610a0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="610a0-116">Application</span></span> | <span data-ttu-id="610a0-117">Calendar.Read, Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="610a0-117">Calendar.Read, Calendar.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="610a0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="610a0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="610a0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="610a0-119">Request headers</span></span>
| <span data-ttu-id="610a0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="610a0-120">Name</span></span>       | <span data-ttu-id="610a0-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="610a0-121">Type</span></span> | <span data-ttu-id="610a0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="610a0-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="610a0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="610a0-123">Authorization</span></span>  | <span data-ttu-id="610a0-124">string</span><span class="sxs-lookup"><span data-stu-id="610a0-124">string</span></span>  | <span data-ttu-id="610a0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="610a0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="610a0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="610a0-127">Content-Type</span></span>  | <span data-ttu-id="610a0-128">string</span><span class="sxs-lookup"><span data-stu-id="610a0-128">string</span></span> | <span data-ttu-id="610a0-129">Natureza dos dados no corpo de uma entidade, que é o aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="610a0-129">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="610a0-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="610a0-130">Required.</span></span>  |
| <span data-ttu-id="610a0-131">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="610a0-131">Prefer: outlook.timezone</span></span> | <span data-ttu-id="610a0-132">string</span><span class="sxs-lookup"><span data-stu-id="610a0-132">string</span></span> | <span data-ttu-id="610a0-133">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="610a0-133">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="610a0-134">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="610a0-134">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="610a0-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="610a0-135">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="610a0-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="610a0-136">Request body</span></span>
<span data-ttu-id="610a0-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="610a0-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="610a0-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="610a0-138">Property</span></span>     | <span data-ttu-id="610a0-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="610a0-139">Type</span></span>   |<span data-ttu-id="610a0-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="610a0-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="610a0-141">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="610a0-141">availabilityViewInterval</span></span>|<span data-ttu-id="610a0-142">String</span><span class="sxs-lookup"><span data-stu-id="610a0-142">String</span></span>|<span data-ttu-id="610a0-143">Representa a duração de um intervalo de tempo em um **availabilityView** na resposta.</span><span class="sxs-lookup"><span data-stu-id="610a0-143">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="610a0-144">O padrão é 30 minutos, mínimo é de 6, máximo é 1440.</span><span class="sxs-lookup"><span data-stu-id="610a0-144">The default is 30 minutes, minimum is 6, maximum is 1440.</span></span> <span data-ttu-id="610a0-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="610a0-145">Optional.</span></span>|
|<span data-ttu-id="610a0-146">endTime</span><span class="sxs-lookup"><span data-stu-id="610a0-146">endTime</span></span>|[<span data-ttu-id="610a0-147">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="610a0-147">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="610a0-148">A data, hora e fuso horário que termina o período.</span><span class="sxs-lookup"><span data-stu-id="610a0-148">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="610a0-149">agendamentos</span><span class="sxs-lookup"><span data-stu-id="610a0-149">schedules</span></span>|<span data-ttu-id="610a0-150">String collection</span><span class="sxs-lookup"><span data-stu-id="610a0-150">String collection</span></span>|<span data-ttu-id="610a0-151">Uma coleção de endereços SMTP de usuários, listas de distribuição ou recursos para obter informações de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="610a0-151">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="610a0-152">startTime</span><span class="sxs-lookup"><span data-stu-id="610a0-152">startTime</span></span>|[<span data-ttu-id="610a0-153">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="610a0-153">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="610a0-154">A data, hora e fuso horário que inicia o período.</span><span class="sxs-lookup"><span data-stu-id="610a0-154">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="610a0-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="610a0-155">Response</span></span>

<span data-ttu-id="610a0-156">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [scheduleInformation](../resources/scheduleinformation.md) para cada objeto no `schedules` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="610a0-156">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="610a0-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="610a0-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="610a0-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="610a0-158">Request</span></span>
<span data-ttu-id="610a0-159">O exemplo a seguir obtém as informações de disponibilidade de dois usuários para a data especificada, a hora e o fuso horário.</span><span class="sxs-lookup"><span data-stu-id="610a0-159">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/getschedule 
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{        
    "schedules": ["AdeleV@contoso.onmicrosoft.com", "AlexW@contoso.OnMicrosoft.com"],
    "startTime": {
        "dateTime": "2018-08-06T09:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "endTime": {
        "dateTime": "2018-08-06T18:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "availabilityViewInterval": "15"
}
```

##### <a name="response"></a><span data-ttu-id="610a0-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="610a0-160">Response</span></span>
<span data-ttu-id="610a0-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="610a0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value":[
        {
            "scheduleId":"AdeleV@contoso.onmicrosoft.com",
            "availabilityView":"222222000022000000000000000000000000",
            "scheduleItems":[
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "subject":"Admininstrators debrief",
                    "location":"Foyer",
                    "start":{
                        "dateTime":"2018-08-06T09:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T10:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                },
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "subject":"Lunch yoga",
                    "location":"Courtyard",
                    "start":{
                        "dateTime":"2018-08-06T11:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T12:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                }
            ],
            "workingHours":{
                "daysOfWeek":[
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime":"08:00:00.0000000",
                "endTime":"17:00:00.0000000",
                "timeZone":{
                    "@odata.type":"#microsoft.graph.customTimeZone",
                    "bias":480,
                    "name":"Customized Time Zone",
                    "standardOffset":{
                        "time":"02:00:00.0000000",
                        "dayOccurrence":1,
                        "dayOfWeek":"sunday",
                        "month":11,
                        "year":0
                    },
                    "daylightOffset":{
                        "daylightBias":-60,
                        "time":"02:00:00.0000000",
                        "dayOccurrence":2,
                        "dayOfWeek":"sunday",
                        "month":3,
                        "year":0
                    }
                }
            }
        },
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
                    "isPrivate":false,
                    "status":"Tentative",
                    "subject":"Admininstrators debrief",
                    "location":"Foyer",
                    "start":{
                        "dateTime":"2018-08-06T09:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T10:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                },
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "subject":"Q4 planning",
                    "location":"Big Bear",
                    "start":{
                        "dateTime":"2018-08-06T11:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T13:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                }
            ],
            "workingHours":{
                "daysOfWeek":[
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime":"08:00:00.0000000",
                "endTime":"17:00:00.0000000",
                "timeZone":{
                    "@odata.type":"#microsoft.graph.customTimeZone",
                    "bias":480,
                    "name":"Customized Time Zone",
                    "standardOffset":{
                        "time":"02:00:00.0000000",
                        "dayOccurrence":1,
                        "dayOfWeek":"sunday",
                        "month":11,
                        "year":0
                    },
                    "daylightOffset":{
                        "daylightBias":-60,
                        "time":"02:00:00.0000000",
                        "dayOccurrence":2,
                        "dayOfWeek":"sunday",
                        "month":3,
                        "year":0
                    }
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
  "description": "calendar: getSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
