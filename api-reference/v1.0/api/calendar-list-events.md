---
title: Listar eventos
description: Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 72c2391e3ab568c56cd6973483042a4d5bd79753
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868646"
---
# <a name="list-events"></a><span data-ttu-id="bb658-104">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="bb658-104">List events</span></span>

<span data-ttu-id="bb658-p102">Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.</span><span class="sxs-lookup"><span data-stu-id="bb658-p102">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="bb658-107">Para obter instâncias de evento expandidas, [obtenha a visualização de calendário](calendar-list-calendarview.md) ou [obtenha as instâncias de um evento](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="bb658-107">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bb658-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb658-108">Permissions</span></span>
<span data-ttu-id="bb658-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb658-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb658-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb658-111">Permission type</span></span>      | <span data-ttu-id="bb658-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb658-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb658-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb658-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bb658-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bb658-114">Calendars.Read</span></span>    |
|<span data-ttu-id="bb658-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb658-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb658-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bb658-116">Calendars.Read</span></span>    |
|<span data-ttu-id="bb658-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb658-117">Application</span></span> | <span data-ttu-id="bb658-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bb658-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb658-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb658-119">HTTP request</span></span>
<span data-ttu-id="bb658-120"><!-- { "blockType": "ignored" } -->Um usuário ou do grupo padrão [calendário](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="bb658-120"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="bb658-121">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="bb658-121">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="bb658-122">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="bb658-122">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bb658-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bb658-123">Optional query parameters</span></span>
<span data-ttu-id="bb658-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bb658-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bb658-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb658-125">Request headers</span></span>
| <span data-ttu-id="bb658-126">Nome</span><span class="sxs-lookup"><span data-stu-id="bb658-126">Name</span></span>       | <span data-ttu-id="bb658-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb658-127">Type</span></span> | <span data-ttu-id="bb658-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb658-128">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="bb658-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb658-129">Authorization</span></span>  | <span data-ttu-id="bb658-130">string</span><span class="sxs-lookup"><span data-stu-id="bb658-130">string</span></span> | <span data-ttu-id="bb658-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb658-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bb658-133">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="bb658-133">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="bb658-134">string</span><span class="sxs-lookup"><span data-stu-id="bb658-134">string</span></span> | <span data-ttu-id="bb658-135">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="bb658-135">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="bb658-136">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="bb658-136">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="bb658-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bb658-137">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb658-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb658-138">Request body</span></span>
<span data-ttu-id="bb658-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb658-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb658-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb658-140">Response</span></span>

<span data-ttu-id="bb658-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb658-141">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb658-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb658-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb658-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb658-143">Request</span></span>
<span data-ttu-id="bb658-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb658-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
##### <a name="response"></a><span data-ttu-id="bb658-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb658-145">Response</span></span>
<span data-ttu-id="bb658-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb658-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
