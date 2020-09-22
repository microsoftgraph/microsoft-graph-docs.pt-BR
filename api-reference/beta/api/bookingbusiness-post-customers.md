---
title: Criar bookingCustomer
description: Criar um novo objeto bookingCustomer.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 69187e27949e66606c26012e0ea10dc2742eeb0f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996595"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="0b665-103">Criar bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="0b665-103">Create bookingCustomer</span></span>

<span data-ttu-id="0b665-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b665-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b665-105">Criar um novo objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="0b665-105">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b665-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b665-106">Permissions</span></span>
<span data-ttu-id="0b665-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b665-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b665-109">Permission type</span></span>      | <span data-ttu-id="0b665-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b665-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b665-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b665-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="0b665-112">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="0b665-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0b665-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b665-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b665-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b665-114">Not supported.</span></span>   |
|<span data-ttu-id="0b665-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b665-115">Application</span></span> | <span data-ttu-id="0b665-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b665-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0b665-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b665-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="0b665-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b665-118">Request headers</span></span>
| <span data-ttu-id="0b665-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0b665-119">Name</span></span>       | <span data-ttu-id="0b665-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b665-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0b665-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b665-121">Authorization</span></span>  | <span data-ttu-id="0b665-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="0b665-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b665-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b665-123">Request body</span></span>
<span data-ttu-id="0b665-124">No corpo da solicitação, forneça uma representação JSON do objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="0b665-124">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="0b665-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b665-125">Response</span></span>
<span data-ttu-id="0b665-126">Se bem-sucedido, este método retorna o `201, Created` código de resposta e o objeto [bookingCustomer](../resources/bookingcustomer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b665-126">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b665-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b665-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b665-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b665-128">Request</span></span>
<span data-ttu-id="0b665-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b665-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0b665-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b665-130">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0b665-131">C#</span><span class="sxs-lookup"><span data-stu-id="0b665-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingcustomer-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b665-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b665-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingcustomer-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b665-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b665-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingcustomer-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0b665-134">No corpo da solicitação, forneça uma representação JSON do objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="0b665-134">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0b665-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b665-135">Response</span></span>
<span data-ttu-id="0b665-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0b665-136">The following is an example of the response.</span></span> <span data-ttu-id="0b665-137">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="0b665-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0b665-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b665-138">All of the properties will be returned from an actual call.</span></span>
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


