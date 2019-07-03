---
title: Criar calendário
description: Use esta API para criar um novo calendário para um usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e6655a4b5c634252b05ad525522b7c43f2ffe890
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35452862"
---
# <a name="create-calendar"></a><span data-ttu-id="2f2ba-103">Criar calendário</span><span class="sxs-lookup"><span data-stu-id="2f2ba-103">Create Calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f2ba-104">Use esta API para criar um novo Calendar para um [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="2f2ba-104">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="2f2ba-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f2ba-105">Permissions</span></span>
<span data-ttu-id="2f2ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f2ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f2ba-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f2ba-108">Permission type</span></span>      | <span data-ttu-id="2f2ba-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f2ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f2ba-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f2ba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2f2ba-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f2ba-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2f2ba-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f2ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f2ba-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f2ba-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2f2ba-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f2ba-114">Application</span></span> | <span data-ttu-id="2f2ba-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f2ba-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f2ba-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f2ba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="2f2ba-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f2ba-117">Request headers</span></span>
| <span data-ttu-id="2f2ba-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f2ba-118">Header</span></span>       | <span data-ttu-id="2f2ba-119">Valor</span><span class="sxs-lookup"><span data-stu-id="2f2ba-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f2ba-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f2ba-120">Authorization</span></span>  | <span data-ttu-id="2f2ba-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f2ba-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2f2ba-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f2ba-123">Content-Type</span></span>  | <span data-ttu-id="2f2ba-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2f2ba-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f2ba-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f2ba-125">Request body</span></span>
<span data-ttu-id="2f2ba-126">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="2f2ba-126">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2f2ba-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f2ba-127">Response</span></span>

<span data-ttu-id="2f2ba-128">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f2ba-128">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f2ba-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f2ba-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f2ba-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f2ba-130">Request</span></span>
<span data-ttu-id="2f2ba-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f2ba-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2f2ba-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f2ba-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2f2ba-133">C#</span><span class="sxs-lookup"><span data-stu-id="2f2ba-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendar-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f2ba-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="2f2ba-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendar-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2f2ba-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2f2ba-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendar-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2f2ba-136">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="2f2ba-136">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2f2ba-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f2ba-137">Response</span></span>
<span data-ttu-id="2f2ba-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f2ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
    "color":"auto",
    "isDefaultCalendar":false,
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
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
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
