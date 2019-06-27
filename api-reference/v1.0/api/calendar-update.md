---
title: Atualizar o calendário
description: 'Atualize as propriedades de um objeto calendar. O calendário pode ser um para um usuário '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 252fa52e8875ae745fa30b77fc7e93ae6820e47f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264726"
---
# <a name="update-calendar"></a><span data-ttu-id="8cee7-104">Atualizar o calendário</span><span class="sxs-lookup"><span data-stu-id="8cee7-104">Update calendar</span></span>

<span data-ttu-id="8cee7-105">Atualize as propriedades de um objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="8cee7-105">Update the properties of of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="8cee7-106">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="8cee7-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="8cee7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8cee7-107">Permissions</span></span>
<span data-ttu-id="8cee7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cee7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cee7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cee7-110">Permission type</span></span>      | <span data-ttu-id="8cee7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8cee7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cee7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cee7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8cee7-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8cee7-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8cee7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cee7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cee7-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8cee7-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8cee7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cee7-116">Application</span></span> | <span data-ttu-id="8cee7-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8cee7-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cee7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cee7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="8cee7-119">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="8cee7-119">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="8cee7-120">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="8cee7-120">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="8cee7-121">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="8cee7-121">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8cee7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cee7-122">Request headers</span></span>
| <span data-ttu-id="8cee7-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8cee7-123">Header</span></span>       | <span data-ttu-id="8cee7-124">Valor</span><span class="sxs-lookup"><span data-stu-id="8cee7-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8cee7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cee7-125">Authorization</span></span>  | <span data-ttu-id="8cee7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cee7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8cee7-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8cee7-128">Content-Type</span></span>  | <span data-ttu-id="8cee7-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cee7-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8cee7-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cee7-131">Request body</span></span>
<span data-ttu-id="8cee7-p106">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8cee7-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8cee7-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cee7-135">Property</span></span>     | <span data-ttu-id="8cee7-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cee7-136">Type</span></span>   |<span data-ttu-id="8cee7-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cee7-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cee7-138">color</span><span class="sxs-lookup"><span data-stu-id="8cee7-138">color</span></span>|<span data-ttu-id="8cee7-139">String</span><span class="sxs-lookup"><span data-stu-id="8cee7-139">String</span></span>|<span data-ttu-id="8cee7-p107">Especifica o tema de cores para distinguir o calendário de outros calendários em uma interface do usuário. Os valores de propriedade são: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="8cee7-p107">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="8cee7-142">name</span><span class="sxs-lookup"><span data-stu-id="8cee7-142">name</span></span>|<span data-ttu-id="8cee7-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cee7-143">String</span></span>|<span data-ttu-id="8cee7-144">O nome do calendário.</span><span class="sxs-lookup"><span data-stu-id="8cee7-144">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="8cee7-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cee7-145">Response</span></span>

<span data-ttu-id="8cee7-146">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cee7-146">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8cee7-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cee7-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8cee7-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cee7-148">Request</span></span>
<span data-ttu-id="8cee7-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cee7-149">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="8cee7-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cee7-150">Response</span></span>
<span data-ttu-id="8cee7-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cee7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8cee7-154">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8cee7-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8cee7-155">C#</span><span class="sxs-lookup"><span data-stu-id="8cee7-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_calendar-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8cee7-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="8cee7-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_calendar-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8cee7-157">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8cee7-157">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_calendar-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/calendar-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/calendar-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/calendar-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
