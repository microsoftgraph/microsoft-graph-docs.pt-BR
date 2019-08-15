---
title: Criar bookingCustomer
description: Criar um novo objeto bookingCustomer.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 2defbe4fec3939a94188123126ab942f43bd86ce
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419507"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="46b12-103">Criar bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="46b12-103">Create bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46b12-104">Criar um novo objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="46b12-104">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="46b12-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="46b12-105">Permissions</span></span>
<span data-ttu-id="46b12-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46b12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46b12-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46b12-108">Permission type</span></span>      | <span data-ttu-id="46b12-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46b12-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46b12-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46b12-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="46b12-111">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="46b12-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="46b12-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46b12-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46b12-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46b12-113">Not supported.</span></span>   |
|<span data-ttu-id="46b12-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46b12-114">Application</span></span> | <span data-ttu-id="46b12-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46b12-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="46b12-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46b12-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="46b12-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46b12-117">Request headers</span></span>
| <span data-ttu-id="46b12-118">Nome</span><span class="sxs-lookup"><span data-stu-id="46b12-118">Name</span></span>       | <span data-ttu-id="46b12-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="46b12-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="46b12-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="46b12-120">Authorization</span></span>  | <span data-ttu-id="46b12-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="46b12-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="46b12-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46b12-122">Request body</span></span>
<span data-ttu-id="46b12-123">No corpo da solicitação, forneça uma representação JSON do objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="46b12-123">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="46b12-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="46b12-124">Response</span></span>
<span data-ttu-id="46b12-125">Se bem-sucedido, este método retorna `201, Created` o código de resposta e o objeto [bookingCustomer](../resources/bookingcustomer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46b12-125">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46b12-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46b12-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46b12-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46b12-127">Request</span></span>
<span data-ttu-id="46b12-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="46b12-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="46b12-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="46b12-129">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="46b12-130">C#</span><span class="sxs-lookup"><span data-stu-id="46b12-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingcustomer-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46b12-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46b12-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingcustomer-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46b12-132">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="46b12-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingcustomer-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="46b12-133">No corpo da solicitação, forneça uma representação JSON do objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="46b12-133">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="46b12-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="46b12-134">Response</span></span>
<span data-ttu-id="46b12-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="46b12-135">The following is an example of the response.</span></span> <span data-ttu-id="46b12-136">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="46b12-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="46b12-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46b12-137">All of the properties will be returned from an actual call.</span></span>
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
