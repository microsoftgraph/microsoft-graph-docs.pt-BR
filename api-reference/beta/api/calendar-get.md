---
title: Obter calendário
description: 'Obtenha as propriedades e as relações de um objeto calendar. O calendário pode ser um para um usuário, '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: a611bfe35991aa7558a890ecede8519677c5e643
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322271"
---
# <a name="get-calendar"></a><span data-ttu-id="67e65-104">Obter calendário</span><span class="sxs-lookup"><span data-stu-id="67e65-104">Get calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67e65-105">Obtenha as propriedades e as relações de um objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="67e65-105">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="67e65-106">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="67e65-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="67e65-107">Há dois cenários em que um aplicativo pode obter o calendário de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="67e65-107">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="67e65-108">Se o aplicativo tem permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="67e65-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="67e65-109">Se o aplicativo tem as [permissões](#permissions) delegadas apropriadas de um usuário e o outro usuário compartilhou um calendário com esse usuário ou concedeu acesso delegado ao usuário.</span><span class="sxs-lookup"><span data-stu-id="67e65-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="67e65-110">Confira os [detalhes e um exemplo](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="67e65-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


## <a name="permissions"></a><span data-ttu-id="67e65-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="67e65-111">Permissions</span></span>
<span data-ttu-id="67e65-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67e65-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67e65-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67e65-114">Permission type</span></span>      | <span data-ttu-id="67e65-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67e65-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67e65-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67e65-116">Delegated (work or school account)</span></span> | <span data-ttu-id="67e65-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="67e65-117">Calendars.Read</span></span>    |
|<span data-ttu-id="67e65-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67e65-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67e65-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="67e65-119">Calendars.Read</span></span>    |
|<span data-ttu-id="67e65-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67e65-120">Application</span></span> | <span data-ttu-id="67e65-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="67e65-121">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="67e65-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67e65-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="67e65-123">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="67e65-123">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="67e65-124">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="67e65-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="67e65-125">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="67e65-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="67e65-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="67e65-126">Optional query parameters</span></span>
<span data-ttu-id="67e65-127">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="67e65-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="67e65-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67e65-128">Request headers</span></span>
| <span data-ttu-id="67e65-129">Nome</span><span class="sxs-lookup"><span data-stu-id="67e65-129">Name</span></span>       | <span data-ttu-id="67e65-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="67e65-130">Type</span></span> | <span data-ttu-id="67e65-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="67e65-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="67e65-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="67e65-132">Authorization</span></span>  | <span data-ttu-id="67e65-133">string</span><span class="sxs-lookup"><span data-stu-id="67e65-133">string</span></span>  | <span data-ttu-id="67e65-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67e65-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67e65-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67e65-136">Request body</span></span>
<span data-ttu-id="67e65-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67e65-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67e65-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="67e65-138">Response</span></span>

<span data-ttu-id="67e65-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67e65-139">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="67e65-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67e65-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67e65-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67e65-141">Request</span></span>
<span data-ttu-id="67e65-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67e65-142">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar
```

##### <a name="response"></a><span data-ttu-id="67e65-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="67e65-143">Response</span></span>
<span data-ttu-id="67e65-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67e65-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
