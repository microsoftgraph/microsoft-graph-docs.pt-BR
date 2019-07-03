---
title: Excluir bookingStaffMember
description: Excluir um membro da equipe no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9f1e9ddc50e4c61c8dd7f228540891266656ca98
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439004"
---
# <a name="delete-bookingstaffmember"></a><span data-ttu-id="28155-103">Excluir bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="28155-103">Delete bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28155-104">Excluir um [membro da equipe](../resources/bookingstaffmember.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="28155-104">Delete a [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="28155-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="28155-105">Permissions</span></span>
<span data-ttu-id="28155-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28155-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28155-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28155-108">Permission type</span></span>      | <span data-ttu-id="28155-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28155-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28155-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28155-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="28155-111">Bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="28155-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="28155-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28155-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28155-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28155-113">Not supported.</span></span>   |
|<span data-ttu-id="28155-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28155-114">Application</span></span> | <span data-ttu-id="28155-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28155-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="28155-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28155-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/staffMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="28155-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28155-117">Request headers</span></span>
| <span data-ttu-id="28155-118">Nome</span><span class="sxs-lookup"><span data-stu-id="28155-118">Name</span></span>       | <span data-ttu-id="28155-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="28155-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="28155-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="28155-120">Authorization</span></span>  | <span data-ttu-id="28155-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="28155-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="28155-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28155-122">Request body</span></span>
<span data-ttu-id="28155-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28155-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="28155-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="28155-124">Response</span></span>
<span data-ttu-id="28155-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28155-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28155-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28155-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28155-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28155-128">Request</span></span>
<span data-ttu-id="28155-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="28155-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="28155-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="28155-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingstaffmember"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/5fae928f-6d2d-417a-ad96-4b0caeb362d6
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="28155-131">C#</span><span class="sxs-lookup"><span data-stu-id="28155-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28155-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="28155-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="28155-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="28155-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28155-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="28155-134">Response</span></span>
<span data-ttu-id="28155-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="28155-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
