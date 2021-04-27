---
title: Atualizar o calendário
description: 'Atualize as propriedades de um objeto calendar. O calendário pode ser um para um usuário '
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4e1bd3897a16a9d75ef53e4450fb5a20e1c5651a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047725"
---
# <a name="update-calendar"></a><span data-ttu-id="85091-104">Atualizar calendário</span><span class="sxs-lookup"><span data-stu-id="85091-104">Update calendar</span></span>

<span data-ttu-id="85091-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85091-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85091-106">Atualize as propriedades de um objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="85091-106">Update the properties of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="85091-107">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="85091-107">The calendar can be one for a [user](../resources/user.md), or the default calendar of a Microsoft 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="85091-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="85091-108">Permissions</span></span>
<span data-ttu-id="85091-109">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="85091-109">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="85091-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85091-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85091-111">Calendário</span><span class="sxs-lookup"><span data-stu-id="85091-111">Calendar</span></span> | <span data-ttu-id="85091-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85091-112">Delegated (work or school account)</span></span> | <span data-ttu-id="85091-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85091-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85091-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85091-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="85091-115">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="85091-115">user calendar</span></span> | <span data-ttu-id="85091-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85091-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="85091-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85091-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="85091-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85091-118">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="85091-119">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="85091-119">group calendar</span></span> | <span data-ttu-id="85091-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85091-120">Group.ReadWrite.All</span></span> | <span data-ttu-id="85091-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85091-121">Not supported.</span></span> | <span data-ttu-id="85091-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85091-122">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="85091-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85091-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="85091-124">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="85091-124">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="85091-125">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="85091-125">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}
```
<span data-ttu-id="85091-126">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="85091-126">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="85091-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85091-127">Request headers</span></span>
| <span data-ttu-id="85091-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85091-128">Header</span></span>       | <span data-ttu-id="85091-129">Valor</span><span class="sxs-lookup"><span data-stu-id="85091-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="85091-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="85091-130">Authorization</span></span>  | <span data-ttu-id="85091-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85091-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="85091-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85091-133">Content-Type</span></span>  | <span data-ttu-id="85091-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85091-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="85091-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85091-136">Request body</span></span>
<span data-ttu-id="85091-p106">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="85091-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="85091-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85091-140">Property</span></span>     | <span data-ttu-id="85091-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="85091-141">Type</span></span>   |<span data-ttu-id="85091-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="85091-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85091-143">color</span><span class="sxs-lookup"><span data-stu-id="85091-143">color</span></span>|<span data-ttu-id="85091-144">String</span><span class="sxs-lookup"><span data-stu-id="85091-144">String</span></span>|<span data-ttu-id="85091-p107">Especifica o tema de cores para distinguir o calendário de outros calendários em uma interface do usuário. Os valores de propriedade são: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="85091-p107">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="85091-147">isDefaultCalendar</span><span class="sxs-lookup"><span data-stu-id="85091-147">isDefaultCalendar</span></span>|<span data-ttu-id="85091-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="85091-148">Boolean</span></span>|<span data-ttu-id="85091-149">True se esse calendário for o calendário padrão do usuário, caso contrário, será false.</span><span class="sxs-lookup"><span data-stu-id="85091-149">True if this calendar is the user's default calendar, false otherwise.</span></span>|
|<span data-ttu-id="85091-150">nome</span><span class="sxs-lookup"><span data-stu-id="85091-150">name</span></span>|<span data-ttu-id="85091-151">String</span><span class="sxs-lookup"><span data-stu-id="85091-151">String</span></span>|<span data-ttu-id="85091-152">O nome do calendário.</span><span class="sxs-lookup"><span data-stu-id="85091-152">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="85091-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="85091-153">Response</span></span>

<span data-ttu-id="85091-154">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85091-154">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="85091-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85091-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85091-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85091-156">Request</span></span>
<span data-ttu-id="85091-157">O exemplo a seguir atualiza o nome do calendário padrão do usuário inscreveu.</span><span class="sxs-lookup"><span data-stu-id="85091-157">The following example updates the name of the signed-in user's default calendar.</span></span>

# <a name="http"></a>[<span data-ttu-id="85091-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="85091-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendar"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/calendar
Content-type: application/json

{
  "name": "Social events"
}
```
# <a name="c"></a>[<span data-ttu-id="85091-159">C#</span><span class="sxs-lookup"><span data-stu-id="85091-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85091-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85091-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85091-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85091-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85091-162">Java</span><span class="sxs-lookup"><span data-stu-id="85091-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="85091-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="85091-163">Response</span></span>
<span data-ttu-id="85091-164">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85091-164">Here is an example of the response.</span></span> <span data-ttu-id="85091-165">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="85091-165">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Social events",
    "color":"auto",
    "hexColor": "",
    "isDefaultCalendar":false,
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
    "canShare":true,
    "canViewPrivateItems":true,
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
  "description": "Update calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


