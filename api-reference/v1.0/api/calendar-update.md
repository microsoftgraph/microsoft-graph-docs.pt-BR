---
title: Atualizar o calendário
description: 'Atualize as propriedades de um objeto calendar. O calendário pode ser um para um usuário '
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0c6c17da08557d9026f70c1e9bde987e4c9415a6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070349"
---
# <a name="update-calendar"></a><span data-ttu-id="71039-104">Atualizar calendário</span><span class="sxs-lookup"><span data-stu-id="71039-104">Update calendar</span></span>

<span data-ttu-id="71039-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71039-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71039-106">Atualize as propriedades de um objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="71039-106">Update the properties of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="71039-107">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="71039-107">The calendar can be one for a [user](../resources/user.md), or the default calendar of a Microsoft 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="71039-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="71039-108">Permissions</span></span>
<span data-ttu-id="71039-109">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="71039-109">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="71039-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71039-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71039-111">Calendário</span><span class="sxs-lookup"><span data-stu-id="71039-111">Calendar</span></span> | <span data-ttu-id="71039-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71039-112">Delegated (work or school account)</span></span> | <span data-ttu-id="71039-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71039-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71039-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71039-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="71039-115">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="71039-115">user calendar</span></span> | <span data-ttu-id="71039-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71039-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="71039-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71039-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="71039-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71039-118">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="71039-119">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="71039-119">group calendar</span></span> | <span data-ttu-id="71039-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71039-120">Group.ReadWrite.All</span></span> | <span data-ttu-id="71039-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71039-121">Not supported.</span></span> | <span data-ttu-id="71039-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71039-122">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="71039-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71039-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="71039-124">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="71039-124">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="71039-125">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="71039-125">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="71039-126">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="71039-126">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="71039-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71039-127">Request headers</span></span>
| <span data-ttu-id="71039-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71039-128">Header</span></span>       | <span data-ttu-id="71039-129">Valor</span><span class="sxs-lookup"><span data-stu-id="71039-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="71039-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="71039-130">Authorization</span></span>  | <span data-ttu-id="71039-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71039-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="71039-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71039-133">Content-Type</span></span>  | <span data-ttu-id="71039-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71039-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71039-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71039-136">Request body</span></span>
<span data-ttu-id="71039-p106">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="71039-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="71039-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71039-140">Property</span></span>     | <span data-ttu-id="71039-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="71039-141">Type</span></span>   |<span data-ttu-id="71039-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="71039-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71039-143">color</span><span class="sxs-lookup"><span data-stu-id="71039-143">color</span></span>|<span data-ttu-id="71039-144">String</span><span class="sxs-lookup"><span data-stu-id="71039-144">String</span></span>|<span data-ttu-id="71039-p107">Especifica o tema de cores para distinguir o calendário de outros calendários em uma interface do usuário. Os valores de propriedade são: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="71039-p107">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="71039-147">nome</span><span class="sxs-lookup"><span data-stu-id="71039-147">name</span></span>|<span data-ttu-id="71039-148">String</span><span class="sxs-lookup"><span data-stu-id="71039-148">String</span></span>|<span data-ttu-id="71039-149">O nome do calendário.</span><span class="sxs-lookup"><span data-stu-id="71039-149">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="71039-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="71039-150">Response</span></span>

<span data-ttu-id="71039-151">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71039-151">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71039-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71039-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="71039-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71039-153">Request</span></span>
<span data-ttu-id="71039-154">O exemplo a seguir atualiza o nome do calendário padrão do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="71039-154">The following example updates the name of the signed-in user's default calendar.</span></span>

# <a name="http"></a>[<span data-ttu-id="71039-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="71039-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendar"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/calendar
Content-type: application/json

{
  "name": "Social events"
}
```
# <a name="c"></a>[<span data-ttu-id="71039-156">C#</span><span class="sxs-lookup"><span data-stu-id="71039-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71039-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71039-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71039-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71039-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71039-159">Java</span><span class="sxs-lookup"><span data-stu-id="71039-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="71039-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="71039-160">Response</span></span>
<span data-ttu-id="71039-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71039-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Social events",
    "color":"auto",
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
    "canShare":true,
    "canViewPrivateItems":true,
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
  "description": "Update calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

