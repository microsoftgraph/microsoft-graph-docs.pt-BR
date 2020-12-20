---
title: Obter calendário
description: 'Obtenha as propriedades e as relações de um objeto calendário. O calendário pode ser um para um usuário '
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a66058dd7af69a9e85e241dbc8f35f5b123a9598
ms.sourcegitcommit: 0cde389d4d6dbec1568dab14490f0fd6297d5aa4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720684"
---
# <a name="get-calendar"></a><span data-ttu-id="119bc-104">Obter calendário</span><span class="sxs-lookup"><span data-stu-id="119bc-104">Get calendar</span></span>

<span data-ttu-id="119bc-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="119bc-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="119bc-106">Obtenha as propriedades e as relações de um objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="119bc-106">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="119bc-107">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="119bc-107">The calendar can be one for a [user](../resources/user.md), or the default calendar of a Microsoft 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="119bc-108">Existem dois cenários em que um aplicativo pode receber o calendário de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="119bc-108">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="119bc-109">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="119bc-109">If the app has application permissions, or,</span></span>
* <span data-ttu-id="119bc-110">Se o aplicativo tem as [permissões](#permissions) delegadas apropriadas de um usuário e o outro usuário compartilhou um calendário com esse usuário ou concedeu acesso delegado ao usuário.</span><span class="sxs-lookup"><span data-stu-id="119bc-110">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="119bc-111">Confira [detalhes e um exemplo](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="119bc-111">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

## <a name="permissions"></a><span data-ttu-id="119bc-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="119bc-112">Permissions</span></span>
<span data-ttu-id="119bc-113">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="119bc-113">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="119bc-114">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="119bc-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="119bc-115">Calendário</span><span class="sxs-lookup"><span data-stu-id="119bc-115">Calendar</span></span> | <span data-ttu-id="119bc-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="119bc-116">Delegated (work or school account)</span></span> | <span data-ttu-id="119bc-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="119bc-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="119bc-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="119bc-118">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="119bc-119">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="119bc-119">user calendar</span></span> | <span data-ttu-id="119bc-120">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="119bc-120">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="119bc-121">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="119bc-121">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="119bc-122">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="119bc-122">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="119bc-123">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="119bc-123">group calendar</span></span> | <span data-ttu-id="119bc-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="119bc-124">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="119bc-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="119bc-125">Not supported.</span></span> | <span data-ttu-id="119bc-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="119bc-126">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="119bc-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="119bc-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="119bc-128">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="119bc-128">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="119bc-129">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="119bc-129">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="119bc-130">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="119bc-130">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="119bc-131">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="119bc-131">Optional query parameters</span></span>
<span data-ttu-id="119bc-132">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="119bc-132">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="119bc-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="119bc-133">Request headers</span></span>
| <span data-ttu-id="119bc-134">Nome</span><span class="sxs-lookup"><span data-stu-id="119bc-134">Name</span></span>       | <span data-ttu-id="119bc-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="119bc-135">Type</span></span> | <span data-ttu-id="119bc-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="119bc-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="119bc-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="119bc-137">Authorization</span></span>  | <span data-ttu-id="119bc-138">string</span><span class="sxs-lookup"><span data-stu-id="119bc-138">string</span></span>  | <span data-ttu-id="119bc-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="119bc-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="119bc-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="119bc-141">Request body</span></span>
<span data-ttu-id="119bc-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="119bc-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="119bc-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="119bc-143">Response</span></span>

<span data-ttu-id="119bc-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="119bc-144">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="119bc-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="119bc-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="119bc-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="119bc-146">Request</span></span>
<span data-ttu-id="119bc-147">O exemplo a seguir obtém o calendário padrão do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="119bc-147">The following example gets the signed-in user's default calendar.</span></span>

# <a name="http"></a>[<span data-ttu-id="119bc-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="119bc-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar
```
# <a name="c"></a>[<span data-ttu-id="119bc-149">C#</span><span class="sxs-lookup"><span data-stu-id="119bc-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="119bc-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="119bc-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="119bc-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="119bc-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="119bc-152">Java</span><span class="sxs-lookup"><span data-stu-id="119bc-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="119bc-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="119bc-153">Response</span></span>
<span data-ttu-id="119bc-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="119bc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "isDefaultCalendar": false,
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
    "canShare":true,
    "canViewPrivateItems":true,
    "hexColor": "",
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
<!-- {
  "type": "#page.annotation",
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
