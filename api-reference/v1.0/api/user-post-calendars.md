---
title: Criar calendário
description: Use esta API para criar um novo calendário para um usuário.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 55bf900de03fb278ff4d76c4de4b1e07403d5156
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272972"
---
# <a name="create-calendar"></a><span data-ttu-id="cbbb2-103">Criar calendário</span><span class="sxs-lookup"><span data-stu-id="cbbb2-103">Create Calendar</span></span>

<span data-ttu-id="cbbb2-104">Use esta API para criar um novo Calendar para um [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="cbbb2-104">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="cbbb2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cbbb2-105">Permissions</span></span>
<span data-ttu-id="cbbb2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbbb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbbb2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbbb2-108">Permission type</span></span>      | <span data-ttu-id="cbbb2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbbb2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbbb2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbbb2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cbbb2-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbbb2-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cbbb2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbbb2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbbb2-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbbb2-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cbbb2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbbb2-114">Application</span></span> | <span data-ttu-id="cbbb2-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbbb2-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbbb2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbbb2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="cbbb2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbbb2-117">Request headers</span></span>
| <span data-ttu-id="cbbb2-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cbbb2-118">Header</span></span>       | <span data-ttu-id="cbbb2-119">Valor</span><span class="sxs-lookup"><span data-stu-id="cbbb2-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cbbb2-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbbb2-120">Authorization</span></span>  | <span data-ttu-id="cbbb2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbbb2-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cbbb2-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cbbb2-123">Content-Type</span></span>  | <span data-ttu-id="cbbb2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cbbb2-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cbbb2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbbb2-125">Request body</span></span>
<span data-ttu-id="cbbb2-126">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="cbbb2-126">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cbbb2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbbb2-127">Response</span></span>

<span data-ttu-id="cbbb2-128">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbbb2-128">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbbb2-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbbb2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cbbb2-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbbb2-130">Request</span></span>
<span data-ttu-id="cbbb2-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbbb2-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}
```
<span data-ttu-id="cbbb2-132">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="cbbb2-132">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cbbb2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbbb2-133">Response</span></span>
<span data-ttu-id="cbbb2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbbb2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="cbbb2-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="cbbb2-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cbbb2-138">C#</span><span class="sxs-lookup"><span data-stu-id="cbbb2-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_calendar_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cbbb2-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="cbbb2-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_calendar_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cbbb2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cbbb2-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_calendar_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-post-calendars.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-post-calendars.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-post-calendars.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
