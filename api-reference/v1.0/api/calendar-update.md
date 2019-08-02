---
title: Atualizar o calendário
description: 'Atualize as propriedades de um objeto calendar. O calendário pode ser um para um usuário '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a07b4f901f3a25c370411765698374cd415d19ba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003970"
---
# <a name="update-calendar"></a><span data-ttu-id="1e13e-104">Atualizar calendário</span><span class="sxs-lookup"><span data-stu-id="1e13e-104">Update calendar</span></span>

<span data-ttu-id="1e13e-105">Atualize as propriedades de um objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="1e13e-105">Update the properties of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="1e13e-106">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="1e13e-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="1e13e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e13e-107">Permissions</span></span>
<span data-ttu-id="1e13e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e13e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e13e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e13e-110">Permission type</span></span>      | <span data-ttu-id="1e13e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e13e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e13e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e13e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1e13e-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e13e-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1e13e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e13e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e13e-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e13e-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1e13e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e13e-116">Application</span></span> | <span data-ttu-id="1e13e-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e13e-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e13e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e13e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="1e13e-119">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="1e13e-119">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="1e13e-120">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="1e13e-120">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="1e13e-121">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="1e13e-121">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1e13e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e13e-122">Request headers</span></span>
| <span data-ttu-id="1e13e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e13e-123">Header</span></span>       | <span data-ttu-id="1e13e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="1e13e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1e13e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e13e-125">Authorization</span></span>  | <span data-ttu-id="1e13e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e13e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1e13e-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1e13e-128">Content-Type</span></span>  | <span data-ttu-id="1e13e-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e13e-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1e13e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e13e-131">Request body</span></span>
<span data-ttu-id="1e13e-p106">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1e13e-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1e13e-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e13e-135">Property</span></span>     | <span data-ttu-id="1e13e-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e13e-136">Type</span></span>   |<span data-ttu-id="1e13e-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e13e-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e13e-138">color</span><span class="sxs-lookup"><span data-stu-id="1e13e-138">color</span></span>|<span data-ttu-id="1e13e-139">String</span><span class="sxs-lookup"><span data-stu-id="1e13e-139">String</span></span>|<span data-ttu-id="1e13e-p107">Especifica o tema de cores para distinguir o calendário de outros calendários em uma interface do usuário. Os valores de propriedade são: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="1e13e-p107">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="1e13e-142">name</span><span class="sxs-lookup"><span data-stu-id="1e13e-142">name</span></span>|<span data-ttu-id="1e13e-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e13e-143">String</span></span>|<span data-ttu-id="1e13e-144">O nome do calendário.</span><span class="sxs-lookup"><span data-stu-id="1e13e-144">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="1e13e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e13e-145">Response</span></span>

<span data-ttu-id="1e13e-146">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e13e-146">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1e13e-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e13e-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e13e-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e13e-148">Request</span></span>
<span data-ttu-id="1e13e-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e13e-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1e13e-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e13e-150">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1e13e-151">C#</span><span class="sxs-lookup"><span data-stu-id="1e13e-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e13e-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="1e13e-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1e13e-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1e13e-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1e13e-154">Java</span><span class="sxs-lookup"><span data-stu-id="1e13e-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1e13e-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e13e-155">Response</span></span>
<span data-ttu-id="1e13e-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e13e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
