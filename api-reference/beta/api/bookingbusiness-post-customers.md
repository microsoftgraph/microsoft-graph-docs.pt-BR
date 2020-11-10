---
title: Criar bookingCustomer
description: Criar um novo objeto bookingCustomer.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: a8e89c3b33acbb69a34e66cb55be2d271a9c0cbf
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960681"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="d9968-103">Criar bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="d9968-103">Create bookingCustomer</span></span>

<span data-ttu-id="d9968-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9968-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9968-105">Criar um novo objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="d9968-105">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d9968-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9968-106">Permissions</span></span>
<span data-ttu-id="d9968-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9968-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9968-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9968-109">Permission type</span></span>      | <span data-ttu-id="d9968-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9968-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9968-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9968-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="d9968-112">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="d9968-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d9968-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9968-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9968-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9968-114">Not supported.</span></span>   |
|<span data-ttu-id="d9968-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9968-115">Application</span></span> | <span data-ttu-id="d9968-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9968-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d9968-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9968-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="d9968-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9968-118">Request headers</span></span>
| <span data-ttu-id="d9968-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d9968-119">Name</span></span>       | <span data-ttu-id="d9968-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9968-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d9968-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9968-121">Authorization</span></span>  | <span data-ttu-id="d9968-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d9968-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9968-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9968-123">Request body</span></span>
<span data-ttu-id="d9968-124">No corpo da solicitação, forneça uma representação JSON do objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="d9968-124">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="d9968-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9968-125">Response</span></span>
<span data-ttu-id="d9968-126">Se bem-sucedido, este método retorna o `201, Created` código de resposta e o objeto [bookingCustomer](../resources/bookingcustomer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9968-126">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9968-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9968-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9968-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9968-128">Request</span></span>
<span data-ttu-id="d9968-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9968-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9968-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9968-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_bookingcustomer_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
Content-type: application/json

{
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```
# <a name="c"></a>[<span data-ttu-id="d9968-131">C#</span><span class="sxs-lookup"><span data-stu-id="d9968-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingcustomer-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9968-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9968-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingcustomer-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9968-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9968-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingcustomer-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9968-134">Java</span><span class="sxs-lookup"><span data-stu-id="d9968-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookingcustomer-from-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d9968-135">No corpo da solicitação, forneça uma representação JSON do objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="d9968-135">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d9968-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9968-136">Response</span></span>
<span data-ttu-id="d9968-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9968-137">The following is an example of the response.</span></span> <span data-ttu-id="d9968-138">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="d9968-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d9968-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9968-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "36038f36-634e-44e4-9415-d7d59c2347aa",
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


