---
title: Obter bookingCustomer
description: Obtenha as propriedades e os relacionamentos de um objeto bookingCustomer.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6501603add6a4df4a3e031e37e1ca1a96fb20a14
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865365"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="55a67-103">Obter bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="55a67-103">Get bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55a67-104">Obtenha as propriedades e os relacionamentos de um objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="55a67-104">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="55a67-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="55a67-105">Permissions</span></span>
<span data-ttu-id="55a67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55a67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55a67-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55a67-108">Permission type</span></span>      | <span data-ttu-id="55a67-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55a67-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55a67-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55a67-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="55a67-111">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="55a67-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="55a67-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55a67-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55a67-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55a67-113">Not supported.</span></span>   |
|<span data-ttu-id="55a67-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55a67-114">Application</span></span> | <span data-ttu-id="55a67-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55a67-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="55a67-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55a67-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="55a67-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="55a67-117">Optional query parameters</span></span>
<span data-ttu-id="55a67-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="55a67-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55a67-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55a67-119">Request headers</span></span>
| <span data-ttu-id="55a67-120">Nome</span><span class="sxs-lookup"><span data-stu-id="55a67-120">Name</span></span>      |<span data-ttu-id="55a67-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="55a67-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="55a67-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="55a67-122">Authorization</span></span>  | <span data-ttu-id="55a67-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="55a67-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="55a67-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55a67-124">Request body</span></span>
<span data-ttu-id="55a67-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55a67-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="55a67-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="55a67-126">Response</span></span>
<span data-ttu-id="55a67-127">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingCustomer](../resources/bookingcustomer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55a67-127">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="55a67-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55a67-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55a67-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55a67-129">Request</span></span>
<span data-ttu-id="55a67-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55a67-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="55a67-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="55a67-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="55a67-132">C#</span><span class="sxs-lookup"><span data-stu-id="55a67-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55a67-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="55a67-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="55a67-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="55a67-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="55a67-135">Java</span><span class="sxs-lookup"><span data-stu-id="55a67-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingcustomer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="55a67-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="55a67-136">Response</span></span>
<span data-ttu-id="55a67-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55a67-137">The following is an example of the response.</span></span> <span data-ttu-id="55a67-138">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="55a67-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="55a67-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55a67-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
    "displayName": "Adele Vance",
    "emailAddress": "adelev@proseware.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
