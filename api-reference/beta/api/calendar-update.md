---
title: Atualizar o calendário
description: 'Atualize as propriedades de um objeto calendar. O calendário pode ser uma para um usuário, '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 2fb6ea839d6565c379c2d9af55920bd0166a7fb1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508472"
---
# <a name="update-calendar"></a><span data-ttu-id="592c3-104">Atualizar o calendário</span><span class="sxs-lookup"><span data-stu-id="592c3-104">Update calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="592c3-105">Atualize as propriedades de um objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="592c3-105">Update the properties of of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="592c3-106">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="592c3-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="592c3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="592c3-107">Permissions</span></span>
<span data-ttu-id="592c3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="592c3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="592c3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="592c3-110">Permission type</span></span>      | <span data-ttu-id="592c3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="592c3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="592c3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="592c3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="592c3-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="592c3-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="592c3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="592c3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="592c3-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="592c3-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="592c3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="592c3-116">Application</span></span> | <span data-ttu-id="592c3-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="592c3-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="592c3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="592c3-118">HTTP request</span></span>
<span data-ttu-id="592c3-119"><!-- { "blockType": "ignored" } -->Um usuário ou do grupo padrão [calendário](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="592c3-119"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="592c3-120">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="592c3-120">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="592c3-121">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="592c3-121">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="592c3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="592c3-122">Request headers</span></span>
| <span data-ttu-id="592c3-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="592c3-123">Header</span></span>       | <span data-ttu-id="592c3-124">Valor</span><span class="sxs-lookup"><span data-stu-id="592c3-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="592c3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="592c3-125">Authorization</span></span>  | <span data-ttu-id="592c3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="592c3-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="592c3-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="592c3-128">Content-Type</span></span>  | <span data-ttu-id="592c3-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="592c3-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="592c3-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="592c3-131">Request body</span></span>
<span data-ttu-id="592c3-p106">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="592c3-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="592c3-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="592c3-135">Property</span></span>     | <span data-ttu-id="592c3-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="592c3-136">Type</span></span>   |<span data-ttu-id="592c3-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="592c3-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="592c3-138">color</span><span class="sxs-lookup"><span data-stu-id="592c3-138">color</span></span>|<span data-ttu-id="592c3-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="592c3-139">String</span></span>|<span data-ttu-id="592c3-p107">Especifica o tema de cores para distinguir o calendário de outros calendários em uma interface do usuário. Os valores de propriedade são: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="592c3-p107">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="592c3-142">isDefaultCalendar</span><span class="sxs-lookup"><span data-stu-id="592c3-142">isDefaultCalendar</span></span>|<span data-ttu-id="592c3-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="592c3-143">Boolean</span></span>|<span data-ttu-id="592c3-144">True se este for padrão calendário do usuário, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="592c3-144">True if this calendar is the user's default calendar, false otherwise.</span></span>|
|<span data-ttu-id="592c3-145">name</span><span class="sxs-lookup"><span data-stu-id="592c3-145">name</span></span>|<span data-ttu-id="592c3-146">String</span><span class="sxs-lookup"><span data-stu-id="592c3-146">String</span></span>|<span data-ttu-id="592c3-147">O nome do calendário.</span><span class="sxs-lookup"><span data-stu-id="592c3-147">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="592c3-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="592c3-148">Response</span></span>

<span data-ttu-id="592c3-149">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="592c3-149">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="592c3-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="592c3-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="592c3-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="592c3-151">Request</span></span>
<span data-ttu-id="592c3-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="592c3-152">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="592c3-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="592c3-153">Response</span></span>
<span data-ttu-id="592c3-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="592c3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/calendar-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
