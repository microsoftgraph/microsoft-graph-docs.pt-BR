---
title: Obter calendário
description: 'Obtenha as propriedades e as relações de um objeto calendário. O calendário pode ser um para um usuário '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 847208d0a2b523b9bb0cc947dfe2d0c68b905bab
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262458"
---
# <a name="get-calendar"></a><span data-ttu-id="24174-104">Obter calendário</span><span class="sxs-lookup"><span data-stu-id="24174-104">Get calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24174-105">Obtenha as propriedades e as relações de um objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="24174-105">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="24174-106">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="24174-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="24174-107">Existem dois cenários em que um aplicativo pode receber o calendário de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="24174-107">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="24174-108">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="24174-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="24174-109">Se o aplicativo tem as [permissões](#permissions) delegadas apropriadas de um usuário e o outro usuário compartilhou um calendário com esse usuário ou concedeu acesso delegado ao usuário.</span><span class="sxs-lookup"><span data-stu-id="24174-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="24174-110">Confira [detalhes e um exemplo](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="24174-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


## <a name="permissions"></a><span data-ttu-id="24174-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="24174-111">Permissions</span></span>
<span data-ttu-id="24174-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24174-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24174-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24174-114">Permission type</span></span>      | <span data-ttu-id="24174-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24174-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24174-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24174-116">Delegated (work or school account)</span></span> | <span data-ttu-id="24174-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="24174-117">Calendars.Read</span></span>    |
|<span data-ttu-id="24174-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24174-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24174-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="24174-119">Calendars.Read</span></span>    |
|<span data-ttu-id="24174-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24174-120">Application</span></span> | <span data-ttu-id="24174-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="24174-121">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="24174-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24174-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="24174-123">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="24174-123">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="24174-124">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="24174-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="24174-125">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="24174-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="24174-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="24174-126">Optional query parameters</span></span>
<span data-ttu-id="24174-127">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="24174-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="24174-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24174-128">Request headers</span></span>
| <span data-ttu-id="24174-129">Nome</span><span class="sxs-lookup"><span data-stu-id="24174-129">Name</span></span>       | <span data-ttu-id="24174-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="24174-130">Type</span></span> | <span data-ttu-id="24174-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="24174-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="24174-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="24174-132">Authorization</span></span>  | <span data-ttu-id="24174-133">string</span><span class="sxs-lookup"><span data-stu-id="24174-133">string</span></span>  | <span data-ttu-id="24174-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24174-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24174-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24174-136">Request body</span></span>
<span data-ttu-id="24174-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24174-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24174-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="24174-138">Response</span></span>

<span data-ttu-id="24174-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24174-139">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="24174-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24174-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24174-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24174-141">Request</span></span>
<span data-ttu-id="24174-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24174-142">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar
```

##### <a name="response"></a><span data-ttu-id="24174-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="24174-143">Response</span></span>
<span data-ttu-id="24174-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24174-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#me/calendars/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
    "id": "AAMkAGI2TGuLAAA=",
    "name": "Calendar",
    "color": "auto",
    "isDefaultCalendar": false,
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
    "canShare":true,
    "canViewPrivateItems":true,
    "hexColor": "",
    "isShared":false,
    "isSharedWithMe":false,
    "canEdit":true,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
    }
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="24174-147">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="24174-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="24174-148">C#</span><span class="sxs-lookup"><span data-stu-id="24174-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_calendar-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24174-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="24174-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_calendar-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="24174-150">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="24174-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_calendar-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/calendar-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/calendar-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/calendar-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
