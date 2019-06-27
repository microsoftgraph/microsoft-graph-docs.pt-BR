---
title: Excluir bookingStaffMember
description: Excluir um membro da equipe no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: e494943dd547bdee4809b5026e26082490f7e2c1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262493"
---
# <a name="delete-bookingstaffmember"></a><span data-ttu-id="c5783-103">Excluir bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="c5783-103">Delete bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5783-104">Excluir um [membro da equipe](../resources/bookingstaffmember.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="c5783-104">Delete a [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c5783-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5783-105">Permissions</span></span>
<span data-ttu-id="c5783-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5783-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5783-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5783-108">Permission type</span></span>      | <span data-ttu-id="c5783-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5783-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5783-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5783-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c5783-111">Bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="c5783-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c5783-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5783-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5783-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5783-113">Not supported.</span></span>   |
|<span data-ttu-id="c5783-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5783-114">Application</span></span> | <span data-ttu-id="c5783-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5783-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c5783-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5783-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/staffMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c5783-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5783-117">Request headers</span></span>
| <span data-ttu-id="c5783-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c5783-118">Name</span></span>       | <span data-ttu-id="c5783-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5783-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c5783-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5783-120">Authorization</span></span>  | <span data-ttu-id="c5783-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="c5783-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5783-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5783-122">Request body</span></span>
<span data-ttu-id="c5783-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5783-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c5783-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5783-124">Response</span></span>
<span data-ttu-id="c5783-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5783-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5783-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5783-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5783-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5783-128">Request</span></span>
<span data-ttu-id="c5783-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5783-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingstaffmember"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/5fae928f-6d2d-417a-ad96-4b0caeb362d6
```
##### <a name="response"></a><span data-ttu-id="c5783-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5783-130">Response</span></span>
<span data-ttu-id="c5783-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c5783-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c5783-132">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="c5783-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c5783-133">C#</span><span class="sxs-lookup"><span data-stu-id="c5783-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_bookingstaffmember-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c5783-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="c5783-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_bookingstaffmember-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c5783-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c5783-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_bookingstaffmember-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingstaffmember-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingstaffmember-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingstaffmember-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
