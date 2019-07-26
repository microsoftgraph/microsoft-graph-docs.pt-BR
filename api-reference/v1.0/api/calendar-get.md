---
title: Obter calendário
description: 'Obtenha as propriedades e as relações de um objeto calendário. O calendário pode ser um para um usuário '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: cb26ceb1d75814919f8d796eb10b2848fdb6f034
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882460"
---
# <a name="get-calendar"></a><span data-ttu-id="543d4-104">Obter calendário</span><span class="sxs-lookup"><span data-stu-id="543d4-104">Get calendar</span></span>

<span data-ttu-id="543d4-105">Obtenha as propriedades e as relações de um objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="543d4-105">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="543d4-106">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="543d4-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="543d4-107">Existem dois cenários em que um aplicativo pode receber o calendário de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="543d4-107">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="543d4-108">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="543d4-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="543d4-109">Se o aplicativo tem as [permissões](#permissions) delegadas apropriadas de um usuário e o outro usuário compartilhou um calendário com esse usuário ou concedeu acesso delegado ao usuário.</span><span class="sxs-lookup"><span data-stu-id="543d4-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="543d4-110">Confira [detalhes e um exemplo](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="543d4-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

## <a name="permissions"></a><span data-ttu-id="543d4-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="543d4-111">Permissions</span></span>
<span data-ttu-id="543d4-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="543d4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="543d4-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="543d4-114">Permission type</span></span>      | <span data-ttu-id="543d4-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="543d4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="543d4-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="543d4-116">Delegated (work or school account)</span></span> | <span data-ttu-id="543d4-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="543d4-117">Calendars.Read</span></span>    |
|<span data-ttu-id="543d4-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="543d4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="543d4-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="543d4-119">Calendars.Read</span></span>    |
|<span data-ttu-id="543d4-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="543d4-120">Application</span></span> | <span data-ttu-id="543d4-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="543d4-121">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="543d4-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="543d4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="543d4-123">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="543d4-123">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="543d4-124">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="543d4-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="543d4-125">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="543d4-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="543d4-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="543d4-126">Optional query parameters</span></span>
<span data-ttu-id="543d4-127">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="543d4-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="543d4-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="543d4-128">Request headers</span></span>
| <span data-ttu-id="543d4-129">Nome</span><span class="sxs-lookup"><span data-stu-id="543d4-129">Name</span></span>       | <span data-ttu-id="543d4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="543d4-130">Type</span></span> | <span data-ttu-id="543d4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="543d4-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="543d4-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="543d4-132">Authorization</span></span>  | <span data-ttu-id="543d4-133">string</span><span class="sxs-lookup"><span data-stu-id="543d4-133">string</span></span>  | <span data-ttu-id="543d4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="543d4-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="543d4-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="543d4-136">Request body</span></span>
<span data-ttu-id="543d4-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="543d4-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="543d4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="543d4-138">Response</span></span>

<span data-ttu-id="543d4-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="543d4-139">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="543d4-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="543d4-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="543d4-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="543d4-141">Request</span></span>
<span data-ttu-id="543d4-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="543d4-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="543d4-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="543d4-143">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="543d4-144">C#</span><span class="sxs-lookup"><span data-stu-id="543d4-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="543d4-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="543d4-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="543d4-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="543d4-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="543d4-147">Java</span><span class="sxs-lookup"><span data-stu-id="543d4-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="543d4-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="543d4-148">Response</span></span>
<span data-ttu-id="543d4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="543d4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
    "id": "AAMkAGI2TGuLAAA=",
    "name": "Calendar",
    "color": "auto",
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
    "canShare":true,
    "canViewPrivateItems":true,
    "canEdit":true,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
