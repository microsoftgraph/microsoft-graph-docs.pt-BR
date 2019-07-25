---
title: Listar eventos
description: Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f14fe27cf236e8843415d2aa54fb281d6af58dca
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865056"
---
# <a name="list-events"></a><span data-ttu-id="4831d-104">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="4831d-104">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4831d-p102">Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.</span><span class="sxs-lookup"><span data-stu-id="4831d-p102">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="4831d-107">Para obter instâncias de evento expandidas, [obtenha a visualização de calendário](calendar-list-calendarview.md) ou [obtenha as instâncias de um evento](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="4831d-107">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4831d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4831d-108">Permissions</span></span>
<span data-ttu-id="4831d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4831d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4831d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4831d-111">Permission type</span></span>      | <span data-ttu-id="4831d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4831d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4831d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4831d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4831d-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4831d-114">Calendars.Read</span></span>    |
|<span data-ttu-id="4831d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4831d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4831d-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4831d-116">Calendars.Read</span></span>    |
|<span data-ttu-id="4831d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4831d-117">Application</span></span> | <span data-ttu-id="4831d-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4831d-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="4831d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4831d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="4831d-120">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="4831d-120">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="4831d-121">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="4831d-121">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="4831d-122">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="4831d-122">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4831d-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4831d-123">Optional query parameters</span></span>
<span data-ttu-id="4831d-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4831d-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4831d-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4831d-125">Request headers</span></span>
| <span data-ttu-id="4831d-126">Nome</span><span class="sxs-lookup"><span data-stu-id="4831d-126">Name</span></span>       | <span data-ttu-id="4831d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="4831d-127">Type</span></span> | <span data-ttu-id="4831d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="4831d-128">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="4831d-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="4831d-129">Authorization</span></span>  | <span data-ttu-id="4831d-130">string</span><span class="sxs-lookup"><span data-stu-id="4831d-130">string</span></span> | <span data-ttu-id="4831d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4831d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4831d-133">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="4831d-133">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="4831d-134">string</span><span class="sxs-lookup"><span data-stu-id="4831d-134">string</span></span> | <span data-ttu-id="4831d-135">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="4831d-135">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="4831d-136">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="4831d-136">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="4831d-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="4831d-137">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4831d-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4831d-138">Request body</span></span>
<span data-ttu-id="4831d-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4831d-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4831d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4831d-140">Response</span></span>

<span data-ttu-id="4831d-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4831d-141">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4831d-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4831d-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4831d-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4831d-143">Request</span></span>
<span data-ttu-id="4831d-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4831d-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4831d-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4831d-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/events
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4831d-146">C#</span><span class="sxs-lookup"><span data-stu-id="4831d-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4831d-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="4831d-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4831d-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4831d-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4831d-149">Java</span><span class="sxs-lookup"><span data-stu-id="4831d-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendar-get-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4831d-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="4831d-150">Response</span></span>
<span data-ttu-id="4831d-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4831d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
