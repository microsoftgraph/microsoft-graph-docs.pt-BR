---
title: Excluir bookingStaffMember
description: Excluir um membro da equipe no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 5442d72f8c97d69ff91ae7d0747f920077d36e33
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318094"
---
# <a name="delete-bookingstaffmember"></a><span data-ttu-id="9f1db-103">Excluir bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="9f1db-103">Delete bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f1db-104">Excluir um [membro da equipe](../resources/bookingstaffmember.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="9f1db-104">Delete a [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="9f1db-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f1db-105">Permissions</span></span>
<span data-ttu-id="9f1db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f1db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f1db-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f1db-108">Permission type</span></span>      | <span data-ttu-id="9f1db-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f1db-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f1db-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f1db-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="9f1db-111">Bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="9f1db-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9f1db-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f1db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f1db-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f1db-113">Not supported.</span></span>   |
|<span data-ttu-id="9f1db-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f1db-114">Application</span></span> | <span data-ttu-id="9f1db-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f1db-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9f1db-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f1db-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/staffMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9f1db-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f1db-117">Request headers</span></span>
| <span data-ttu-id="9f1db-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9f1db-118">Name</span></span>       | <span data-ttu-id="9f1db-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f1db-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9f1db-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f1db-120">Authorization</span></span>  | <span data-ttu-id="9f1db-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9f1db-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f1db-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f1db-122">Request body</span></span>
<span data-ttu-id="9f1db-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9f1db-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9f1db-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f1db-124">Response</span></span>
<span data-ttu-id="9f1db-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f1db-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f1db-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f1db-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f1db-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f1db-128">Request</span></span>
<span data-ttu-id="9f1db-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f1db-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9f1db-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f1db-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingstaffmember"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/5fae928f-6d2d-417a-ad96-4b0caeb362d6
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9f1db-131">C#</span><span class="sxs-lookup"><span data-stu-id="9f1db-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9f1db-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f1db-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9f1db-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9f1db-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9f1db-134">Java</span><span class="sxs-lookup"><span data-stu-id="9f1db-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingstaffmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9f1db-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f1db-135">Response</span></span>
<span data-ttu-id="9f1db-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f1db-136">The following is an example of the response.</span></span>
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
