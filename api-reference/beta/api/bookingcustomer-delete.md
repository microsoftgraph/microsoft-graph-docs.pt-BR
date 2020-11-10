---
title: Excluir bookingCustomer
description: Exclua o objeto bookingCustomer especificado.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: fec10d65b62e8db29a2947f4afdd8428f031f43b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960499"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="f696e-103">Excluir bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="f696e-103">Delete bookingCustomer</span></span>

<span data-ttu-id="f696e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f696e-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f696e-105">Exclua o objeto [bookingCustomer](../resources/bookingcustomer.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="f696e-105">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f696e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f696e-106">Permissions</span></span>
<span data-ttu-id="f696e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f696e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f696e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f696e-109">Permission type</span></span>      | <span data-ttu-id="f696e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f696e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f696e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f696e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f696e-112">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="f696e-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f696e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f696e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f696e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f696e-114">Not supported.</span></span>   |
|<span data-ttu-id="f696e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f696e-115">Application</span></span> | <span data-ttu-id="f696e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f696e-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f696e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f696e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="f696e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f696e-118">Request headers</span></span>
| <span data-ttu-id="f696e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f696e-119">Name</span></span>       | <span data-ttu-id="f696e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f696e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f696e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f696e-121">Authorization</span></span>  | <span data-ttu-id="f696e-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f696e-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f696e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f696e-123">Request body</span></span>
<span data-ttu-id="f696e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f696e-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f696e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f696e-125">Response</span></span>
<span data-ttu-id="f696e-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f696e-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f696e-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f696e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f696e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f696e-129">Request</span></span>
<span data-ttu-id="f696e-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f696e-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f696e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f696e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
# <a name="c"></a>[<span data-ttu-id="f696e-132">C#</span><span class="sxs-lookup"><span data-stu-id="f696e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f696e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f696e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f696e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f696e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f696e-135">Java</span><span class="sxs-lookup"><span data-stu-id="f696e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingcustomer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f696e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f696e-136">Response</span></span>
<span data-ttu-id="f696e-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f696e-137">The following is an example of the response.</span></span> <span data-ttu-id="f696e-138">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="f696e-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f696e-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f696e-139">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


