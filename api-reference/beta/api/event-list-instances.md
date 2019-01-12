---
title: Listar instâncias
description: Obtenha as instâncias (ocorrências) de um evento para um intervalo de tempo especificado. Se o evento for um `SeriesMaster` digitar, isto retorna o
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7a40e6f468c8541748adbc7d8dd588541318c30c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980927"
---
# <a name="list-instances"></a><span data-ttu-id="728f0-104">Instâncias de lista</span><span class="sxs-lookup"><span data-stu-id="728f0-104">List instances</span></span>

> <span data-ttu-id="728f0-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="728f0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="728f0-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="728f0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="728f0-p103">Obtenha as instâncias (ocorrências) de um evento para um intervalo de tempo especificado. Se o evento for do tipo `SeriesMaster`, isso retornará as exceções e ocorrências do evento no intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="728f0-p103">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="728f0-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="728f0-109">Permissions</span></span>
<span data-ttu-id="728f0-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="728f0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="728f0-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="728f0-112">Permission type</span></span>      | <span data-ttu-id="728f0-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="728f0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="728f0-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="728f0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="728f0-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="728f0-115">Calendars.Read</span></span>    |
|<span data-ttu-id="728f0-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="728f0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="728f0-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="728f0-117">Calendars.Read</span></span>    |
|<span data-ttu-id="728f0-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="728f0-118">Application</span></span> | <span data-ttu-id="728f0-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="728f0-119">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="728f0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="728f0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="728f0-121">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="728f0-121">Query parameters</span></span>

<span data-ttu-id="728f0-122">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="728f0-122">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="728f0-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="728f0-123">Parameter</span></span>    | <span data-ttu-id="728f0-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="728f0-124">Type</span></span>   |<span data-ttu-id="728f0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="728f0-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="728f0-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="728f0-126">startDateTime</span></span>|<span data-ttu-id="728f0-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="728f0-127">String</span></span>|<span data-ttu-id="728f0-p105">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="728f0-p105">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="728f0-130">endDateTime</span><span class="sxs-lookup"><span data-stu-id="728f0-130">endDateTime</span></span>|<span data-ttu-id="728f0-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="728f0-131">String</span></span>|<span data-ttu-id="728f0-p106">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="728f0-p106">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="728f0-134">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="728f0-134">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="728f0-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="728f0-135">Request headers</span></span>
| <span data-ttu-id="728f0-136">Nome</span><span class="sxs-lookup"><span data-stu-id="728f0-136">Name</span></span>       | <span data-ttu-id="728f0-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="728f0-137">Type</span></span> | <span data-ttu-id="728f0-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="728f0-138">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="728f0-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="728f0-139">Authorization</span></span>  | <span data-ttu-id="728f0-140">string</span><span class="sxs-lookup"><span data-stu-id="728f0-140">string</span></span> | <span data-ttu-id="728f0-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="728f0-p107">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="728f0-143">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="728f0-143">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="728f0-144">string</span><span class="sxs-lookup"><span data-stu-id="728f0-144">string</span></span> | <span data-ttu-id="728f0-145">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="728f0-145">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="728f0-146">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="728f0-146">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="728f0-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="728f0-147">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="728f0-148">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="728f0-148">Request body</span></span>
<span data-ttu-id="728f0-149">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="728f0-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="728f0-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="728f0-150">Response</span></span>

<span data-ttu-id="728f0-151">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="728f0-151">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="728f0-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="728f0-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="728f0-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="728f0-153">Request</span></span>
<span data-ttu-id="728f0-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="728f0-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="728f0-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="728f0-155">Response</span></span>
<span data-ttu-id="728f0-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="728f0-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "",
        "time": "2016-10-19T10:37:00Z"
      },
      "uid": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
