---
title: Excluir bookingCustomer
description: Exclua o objeto bookingCustomer especificado.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: e756fda2f750dda0fb75c30fd76f7bc8fbe04779
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43376468"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="d5189-103">Excluir bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="d5189-103">Delete bookingCustomer</span></span>

<span data-ttu-id="d5189-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5189-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5189-105">Exclua o objeto [bookingCustomer](../resources/bookingcustomer.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="d5189-105">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d5189-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5189-106">Permissions</span></span>
<span data-ttu-id="d5189-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5189-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5189-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5189-109">Permission type</span></span>      | <span data-ttu-id="d5189-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5189-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5189-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5189-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d5189-112">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="d5189-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d5189-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5189-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5189-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5189-114">Not supported.</span></span>   |
|<span data-ttu-id="d5189-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5189-115">Application</span></span> | <span data-ttu-id="d5189-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5189-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d5189-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5189-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="d5189-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5189-118">Request headers</span></span>
| <span data-ttu-id="d5189-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d5189-119">Name</span></span>       | <span data-ttu-id="d5189-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5189-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d5189-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5189-121">Authorization</span></span>  | <span data-ttu-id="d5189-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d5189-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5189-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5189-123">Request body</span></span>
<span data-ttu-id="d5189-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d5189-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d5189-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5189-125">Response</span></span>
<span data-ttu-id="d5189-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5189-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5189-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5189-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5189-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5189-129">Request</span></span>
<span data-ttu-id="d5189-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5189-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d5189-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5189-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
# <a name="c"></a>[<span data-ttu-id="d5189-132">C#</span><span class="sxs-lookup"><span data-stu-id="d5189-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5189-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5189-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5189-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5189-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d5189-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5189-135">Response</span></span>
<span data-ttu-id="d5189-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d5189-136">The following is an example of the response.</span></span> <span data-ttu-id="d5189-137">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="d5189-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d5189-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5189-138">All of the properties will be returned from an actual call.</span></span>
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
