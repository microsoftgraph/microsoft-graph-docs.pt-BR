---
title: Excluir bookingCustomer
description: Exclua o objeto bookingCustomer especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 34fc848330b8dd089f395829c82cc040887b5c31
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419395"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="4a2ea-103">Excluir bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="4a2ea-103">Delete bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a2ea-104">Exclua o objeto [bookingCustomer](../resources/bookingcustomer.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-104">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a2ea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a2ea-105">Permissions</span></span>
<span data-ttu-id="4a2ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a2ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a2ea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a2ea-108">Permission type</span></span>      | <span data-ttu-id="4a2ea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a2ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a2ea-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a2ea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4a2ea-111">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="4a2ea-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4a2ea-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a2ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a2ea-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-113">Not supported.</span></span>   |
|<span data-ttu-id="4a2ea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a2ea-114">Application</span></span> | <span data-ttu-id="4a2ea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4a2ea-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a2ea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="4a2ea-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a2ea-117">Request headers</span></span>
| <span data-ttu-id="4a2ea-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4a2ea-118">Name</span></span>       | <span data-ttu-id="4a2ea-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a2ea-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4a2ea-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a2ea-120">Authorization</span></span>  | <span data-ttu-id="4a2ea-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="4a2ea-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a2ea-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a2ea-122">Request body</span></span>
<span data-ttu-id="4a2ea-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4a2ea-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a2ea-124">Response</span></span>
<span data-ttu-id="4a2ea-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a2ea-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a2ea-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a2ea-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a2ea-128">Request</span></span>
<span data-ttu-id="4a2ea-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4a2ea-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a2ea-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4a2ea-131">C#</span><span class="sxs-lookup"><span data-stu-id="4a2ea-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a2ea-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a2ea-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4a2ea-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4a2ea-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4a2ea-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a2ea-134">Response</span></span>
<span data-ttu-id="4a2ea-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-135">The following is an example of the response.</span></span> <span data-ttu-id="4a2ea-136">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4a2ea-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-137">All of the properties will be returned from an actual call.</span></span>
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
