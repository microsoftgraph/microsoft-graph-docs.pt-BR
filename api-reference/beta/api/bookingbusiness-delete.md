---
title: Excluir bookingBusiness
description: Excluir um objeto bookingBusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b4def2ea77facec964ad4960e2c78aac2cb89d8c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945197"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="62d75-103">Excluir bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="62d75-103">Delete bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62d75-104">Excluir um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="62d75-104">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="62d75-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="62d75-105">Permissions</span></span>
<span data-ttu-id="62d75-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62d75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62d75-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62d75-108">Permission type</span></span>      | <span data-ttu-id="62d75-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62d75-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62d75-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62d75-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="62d75-111">Bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="62d75-111">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="62d75-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62d75-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62d75-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62d75-113">Not supported.</span></span>   |
|<span data-ttu-id="62d75-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62d75-114">Application</span></span> | <span data-ttu-id="62d75-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62d75-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="62d75-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62d75-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="62d75-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62d75-117">Request headers</span></span>
| <span data-ttu-id="62d75-118">Nome</span><span class="sxs-lookup"><span data-stu-id="62d75-118">Name</span></span>       | <span data-ttu-id="62d75-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="62d75-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="62d75-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="62d75-120">Authorization</span></span>  | <span data-ttu-id="62d75-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="62d75-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="62d75-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62d75-122">Request body</span></span>
<span data-ttu-id="62d75-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="62d75-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="62d75-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="62d75-124">Response</span></span>
<span data-ttu-id="62d75-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62d75-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62d75-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62d75-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62d75-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62d75-128">Request</span></span>
<span data-ttu-id="62d75-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="62d75-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="62d75-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="62d75-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="62d75-131">C#</span><span class="sxs-lookup"><span data-stu-id="62d75-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62d75-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="62d75-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="62d75-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="62d75-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="62d75-134">Java</span><span class="sxs-lookup"><span data-stu-id="62d75-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="62d75-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="62d75-135">Response</span></span>
<span data-ttu-id="62d75-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="62d75-136">The following is an example of the response.</span></span>
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
  "description": "Delete bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
