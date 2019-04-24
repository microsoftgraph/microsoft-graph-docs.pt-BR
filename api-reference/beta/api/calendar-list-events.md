---
title: Listar eventos
description: Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: b92c9049867891f27fc7d75b3bfe4be8bd3fdb17
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461875"
---
# <a name="list-events"></a><span data-ttu-id="1cb3b-104">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="1cb3b-104">List events</span></span>

<span data-ttu-id="1cb3b-p102">Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-p102">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="1cb3b-107">Para obter instâncias de evento expandidas, [obtenha a visualização de calendário](calendar-list-calendarview.md) ou [obtenha as instâncias de um evento](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="1cb3b-107">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1cb3b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cb3b-108">Permissions</span></span>
<span data-ttu-id="1cb3b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cb3b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cb3b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cb3b-111">Permission type</span></span>      | <span data-ttu-id="1cb3b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cb3b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cb3b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cb3b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1cb3b-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1cb3b-114">Calendars.Read</span></span>    |
|<span data-ttu-id="1cb3b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cb3b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cb3b-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1cb3b-116">Calendars.Read</span></span>    |
|<span data-ttu-id="1cb3b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cb3b-117">Application</span></span> | <span data-ttu-id="1cb3b-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1cb3b-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cb3b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cb3b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="1cb3b-120">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-120">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="1cb3b-121">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-121">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="1cb3b-122">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-122">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1cb3b-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1cb3b-123">Optional query parameters</span></span>
<span data-ttu-id="1cb3b-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1cb3b-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cb3b-125">Request headers</span></span>
| <span data-ttu-id="1cb3b-126">Nome</span><span class="sxs-lookup"><span data-stu-id="1cb3b-126">Name</span></span>       | <span data-ttu-id="1cb3b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cb3b-127">Type</span></span> | <span data-ttu-id="1cb3b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cb3b-128">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="1cb3b-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cb3b-129">Authorization</span></span>  | <span data-ttu-id="1cb3b-130">string</span><span class="sxs-lookup"><span data-stu-id="1cb3b-130">string</span></span> | <span data-ttu-id="1cb3b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1cb3b-133">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="1cb3b-133">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="1cb3b-134">string</span><span class="sxs-lookup"><span data-stu-id="1cb3b-134">string</span></span> | <span data-ttu-id="1cb3b-135">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-135">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="1cb3b-136">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-136">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="1cb3b-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-137">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cb3b-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cb3b-138">Request body</span></span>
<span data-ttu-id="1cb3b-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cb3b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cb3b-140">Response</span></span>

<span data-ttu-id="1cb3b-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-141">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1cb3b-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1cb3b-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1cb3b-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cb3b-143">Request</span></span>
<span data-ttu-id="1cb3b-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
##### <a name="response"></a><span data-ttu-id="1cb3b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cb3b-145">Response</span></span>
<span data-ttu-id="1cb3b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
