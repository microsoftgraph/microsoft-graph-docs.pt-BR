---
title: Obter calendário
description: 'Obtenha as propriedades e as relações de um objeto calendário. O calendário pode ser um para um usuário '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1b016be1611072b7ab0fb3f87b4c1086875172a5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936829"
---
# <a name="get-calendar"></a><span data-ttu-id="3f897-104">Obter calendário</span><span class="sxs-lookup"><span data-stu-id="3f897-104">Get calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f897-105">Obtenha as propriedades e as relações de um objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="3f897-105">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="3f897-106">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="3f897-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="3f897-107">Existem dois cenários em que um aplicativo pode receber o calendário de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="3f897-107">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="3f897-108">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="3f897-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="3f897-109">Se o aplicativo tem as [permissões](#permissions) delegadas apropriadas de um usuário e o outro usuário compartilhou um calendário com esse usuário ou concedeu acesso delegado ao usuário.</span><span class="sxs-lookup"><span data-stu-id="3f897-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="3f897-110">Confira [detalhes e um exemplo](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="3f897-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


## <a name="permissions"></a><span data-ttu-id="3f897-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="3f897-111">Permissions</span></span>
<span data-ttu-id="3f897-112">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="3f897-112">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="3f897-113">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f897-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3f897-114">Calendário</span><span class="sxs-lookup"><span data-stu-id="3f897-114">Calendar</span></span> | <span data-ttu-id="3f897-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f897-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3f897-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f897-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f897-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f897-117">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="3f897-118">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="3f897-118">user calendar</span></span> | <span data-ttu-id="3f897-119">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f897-119">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="3f897-120">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f897-120">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="3f897-121">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f897-121">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="3f897-122">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="3f897-122">group calendar</span></span> | <span data-ttu-id="3f897-123">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f897-123">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="3f897-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f897-124">Not supported.</span></span> | <span data-ttu-id="3f897-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f897-125">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="3f897-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f897-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="3f897-127">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="3f897-127">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="3f897-128">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="3f897-128">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="3f897-129">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="3f897-129">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3f897-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3f897-130">Optional query parameters</span></span>
<span data-ttu-id="3f897-131">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3f897-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3f897-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f897-132">Request headers</span></span>
| <span data-ttu-id="3f897-133">Nome</span><span class="sxs-lookup"><span data-stu-id="3f897-133">Name</span></span>       | <span data-ttu-id="3f897-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f897-134">Type</span></span> | <span data-ttu-id="3f897-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f897-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3f897-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f897-136">Authorization</span></span>  | <span data-ttu-id="3f897-137">string</span><span class="sxs-lookup"><span data-stu-id="3f897-137">string</span></span>  | <span data-ttu-id="3f897-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f897-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f897-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f897-140">Request body</span></span>
<span data-ttu-id="3f897-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3f897-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f897-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f897-142">Response</span></span>

<span data-ttu-id="3f897-143">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f897-143">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3f897-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f897-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f897-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f897-145">Request</span></span>
<span data-ttu-id="3f897-146">O exemplo a seguir obtém o calendário padrão do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="3f897-146">The following example gets the signed-in user's default calendar.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3f897-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f897-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3f897-148">C#</span><span class="sxs-lookup"><span data-stu-id="3f897-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3f897-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f897-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3f897-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f897-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3f897-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f897-151">Response</span></span>
<span data-ttu-id="3f897-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f897-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "allowedOnlineMeetingProviders": [
                "teamsForBusiness"
            ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": false,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
    }
}

```

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
  ]
}
-->
