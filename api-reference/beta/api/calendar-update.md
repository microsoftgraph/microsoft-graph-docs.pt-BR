---
title: Atualizar o calendário
description: 'Atualize as propriedades de um objeto calendar. O calendário pode ser uma para um usuário, '
localization_priority: Normal
ms.openlocfilehash: 48a3dd1630ce28aae1f8749cec7a1a4bbd5d6b83
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814368"
---
# <a name="update-calendar"></a><span data-ttu-id="40e92-104">Atualizar o calendário</span><span class="sxs-lookup"><span data-stu-id="40e92-104">Update calendar</span></span>

> <span data-ttu-id="40e92-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="40e92-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40e92-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="40e92-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="40e92-107">Atualize as propriedades de um objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="40e92-107">Update the properties of of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="40e92-108">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="40e92-108">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="40e92-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="40e92-109">Permissions</span></span>
<span data-ttu-id="40e92-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40e92-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40e92-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40e92-112">Permission type</span></span>      | <span data-ttu-id="40e92-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40e92-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40e92-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40e92-114">Delegated (work or school account)</span></span> | <span data-ttu-id="40e92-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40e92-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="40e92-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40e92-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40e92-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40e92-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="40e92-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40e92-118">Application</span></span> | <span data-ttu-id="40e92-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40e92-119">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="40e92-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40e92-120">HTTP request</span></span>
<span data-ttu-id="40e92-121"><!-- { "blockType": "ignored" } -->Um usuário ou do grupo padrão [calendário](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="40e92-121"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="40e92-122">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="40e92-122">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="40e92-123">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="40e92-123">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="40e92-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40e92-124">Request headers</span></span>
| <span data-ttu-id="40e92-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40e92-125">Header</span></span>       | <span data-ttu-id="40e92-126">Valor</span><span class="sxs-lookup"><span data-stu-id="40e92-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="40e92-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="40e92-127">Authorization</span></span>  | <span data-ttu-id="40e92-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40e92-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="40e92-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40e92-130">Content-Type</span></span>  | <span data-ttu-id="40e92-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40e92-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="40e92-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40e92-133">Request body</span></span>
<span data-ttu-id="40e92-p107">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="40e92-p107">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="40e92-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40e92-137">Property</span></span>     | <span data-ttu-id="40e92-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="40e92-138">Type</span></span>   |<span data-ttu-id="40e92-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="40e92-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40e92-140">color</span><span class="sxs-lookup"><span data-stu-id="40e92-140">color</span></span>|<span data-ttu-id="40e92-141">String</span><span class="sxs-lookup"><span data-stu-id="40e92-141">String</span></span>|<span data-ttu-id="40e92-p108">Especifica o tema de cores para distinguir o calendário de outros calendários em uma interface do usuário. Os valores de propriedade são: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="40e92-p108">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="40e92-144">isDefaultCalendar</span><span class="sxs-lookup"><span data-stu-id="40e92-144">isDefaultCalendar</span></span>|<span data-ttu-id="40e92-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e92-145">Boolean</span></span>|<span data-ttu-id="40e92-146">True se este for padrão calendário do usuário, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="40e92-146">True if this calendar is the user's default calendar, false otherwise.</span></span>|
|<span data-ttu-id="40e92-147">name</span><span class="sxs-lookup"><span data-stu-id="40e92-147">name</span></span>|<span data-ttu-id="40e92-148">String</span><span class="sxs-lookup"><span data-stu-id="40e92-148">String</span></span>|<span data-ttu-id="40e92-149">O nome do calendário.</span><span class="sxs-lookup"><span data-stu-id="40e92-149">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="40e92-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="40e92-150">Response</span></span>

<span data-ttu-id="40e92-151">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40e92-151">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40e92-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40e92-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40e92-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40e92-153">Request</span></span>
<span data-ttu-id="40e92-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40e92-154">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="40e92-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="40e92-155">Response</span></span>
<span data-ttu-id="40e92-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40e92-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
