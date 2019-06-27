---
title: Atualizar CalendarGroup
description: Use esta API para criar um novo CalendarGroup.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 67c03ba7b7b48480d05ee28ae15c7000c8385cbc
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269535"
---
# <a name="create-calendargroup"></a><span data-ttu-id="d6e4b-103">Atualizar CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="d6e4b-103">Create CalendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6e4b-104">Use esta API para criar um novo CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="d6e4b-104">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="d6e4b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6e4b-105">Permissions</span></span>
<span data-ttu-id="d6e4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6e4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6e4b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6e4b-108">Permission type</span></span>      | <span data-ttu-id="d6e4b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6e4b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6e4b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6e4b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d6e4b-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6e4b-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d6e4b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6e4b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6e4b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6e4b-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d6e4b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6e4b-114">Application</span></span> | <span data-ttu-id="d6e4b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6e4b-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6e4b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6e4b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="d6e4b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6e4b-117">Request headers</span></span>
| <span data-ttu-id="d6e4b-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6e4b-118">Header</span></span>       | <span data-ttu-id="d6e4b-119">Valor</span><span class="sxs-lookup"><span data-stu-id="d6e4b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d6e4b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6e4b-120">Authorization</span></span>  | <span data-ttu-id="d6e4b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6e4b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d6e4b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6e4b-123">Content-Type</span></span>  | <span data-ttu-id="d6e4b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d6e4b-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d6e4b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6e4b-125">Request body</span></span>
<span data-ttu-id="d6e4b-126">No corpo da solicitação, forneça uma representação JSON do objeto [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="d6e4b-126">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d6e4b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6e4b-127">Response</span></span>

<span data-ttu-id="d6e4b-128">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [CalendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6e4b-128">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6e4b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6e4b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6e4b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6e4b-130">Request</span></span>
<span data-ttu-id="d6e4b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6e4b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
<span data-ttu-id="d6e4b-132">No corpo da solicitação, forneça uma representação JSON do objeto [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="d6e4b-132">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d6e4b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6e4b-133">Response</span></span>
<span data-ttu-id="d6e4b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6e4b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d6e4b-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d6e4b-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d6e4b-138">C#</span><span class="sxs-lookup"><span data-stu-id="d6e4b-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_calendargroup_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6e4b-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="d6e4b-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_calendargroup_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d6e4b-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d6e4b-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_calendargroup_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-post-calendargroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-post-calendargroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-calendargroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
