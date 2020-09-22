---
title: Excluir bookingBusiness
description: Excluir um objeto bookingBusiness.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 70154bedb9454ca345308063a6ccaf4e0f6f0d64
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988104"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="2ef19-103">Excluir bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="2ef19-103">Delete bookingBusiness</span></span>

<span data-ttu-id="2ef19-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ef19-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ef19-105">Excluir um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="2ef19-105">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2ef19-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ef19-106">Permissions</span></span>
<span data-ttu-id="2ef19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ef19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ef19-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ef19-109">Permission type</span></span>      | <span data-ttu-id="2ef19-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ef19-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ef19-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ef19-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="2ef19-112">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="2ef19-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="2ef19-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ef19-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ef19-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ef19-114">Not supported.</span></span>   |
|<span data-ttu-id="2ef19-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ef19-115">Application</span></span> | <span data-ttu-id="2ef19-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ef19-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="2ef19-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef19-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}

```
## <a name="request-headers"></a><span data-ttu-id="2ef19-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef19-118">Request headers</span></span>
| <span data-ttu-id="2ef19-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2ef19-119">Name</span></span>       | <span data-ttu-id="2ef19-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ef19-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2ef19-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ef19-121">Authorization</span></span>  | <span data-ttu-id="2ef19-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="2ef19-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ef19-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef19-123">Request body</span></span>
<span data-ttu-id="2ef19-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ef19-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2ef19-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef19-125">Response</span></span>
<span data-ttu-id="2ef19-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ef19-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ef19-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ef19-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ef19-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef19-129">Request</span></span>
<span data-ttu-id="2ef19-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ef19-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ef19-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef19-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
# <a name="c"></a>[<span data-ttu-id="2ef19-132">C#</span><span class="sxs-lookup"><span data-stu-id="2ef19-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ef19-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ef19-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ef19-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ef19-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2ef19-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef19-135">Response</span></span>
<span data-ttu-id="2ef19-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2ef19-136">The following is an example of the response.</span></span>
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


