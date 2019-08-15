---
title: Listar clientes
description: Obtenha uma lista de objetos bookingCustomer.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 50b3f02db711de9efd01bb300939072ee88f0e09
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415572"
---
# <a name="list-customers"></a><span data-ttu-id="07842-103">Listar clientes</span><span class="sxs-lookup"><span data-stu-id="07842-103">List customers</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07842-104">Obtenha uma lista de objetos [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="07842-104">Get a list of [bookingCustomer](../resources/bookingcustomer.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="07842-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="07842-105">Permissions</span></span>
<span data-ttu-id="07842-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07842-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07842-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07842-108">Permission type</span></span>      | <span data-ttu-id="07842-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07842-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07842-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07842-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="07842-111">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="07842-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="07842-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07842-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07842-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07842-113">Not supported.</span></span>   |
|<span data-ttu-id="07842-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07842-114">Application</span></span> | <span data-ttu-id="07842-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07842-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="07842-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07842-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="07842-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="07842-117">Optional query parameters</span></span>
<span data-ttu-id="07842-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="07842-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07842-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07842-119">Request headers</span></span>
| <span data-ttu-id="07842-120">Nome</span><span class="sxs-lookup"><span data-stu-id="07842-120">Name</span></span>      |<span data-ttu-id="07842-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="07842-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="07842-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="07842-122">Authorization</span></span>  | <span data-ttu-id="07842-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="07842-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="07842-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07842-124">Request body</span></span>
<span data-ttu-id="07842-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="07842-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="07842-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="07842-126">Response</span></span>
<span data-ttu-id="07842-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [bookingCustomer](../resources/bookingcustomer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07842-127">If successful, this method returns a `200 OK` response code and collection of [bookingCustomer](../resources/bookingcustomer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="07842-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07842-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07842-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07842-129">Request</span></span>
<span data-ttu-id="07842-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="07842-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="07842-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="07842-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_customers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="07842-132">C#</span><span class="sxs-lookup"><span data-stu-id="07842-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-customers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="07842-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07842-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-customers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="07842-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="07842-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-customers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="07842-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="07842-135">Response</span></span>
<span data-ttu-id="07842-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="07842-136">The following is an example of the response.</span></span> <span data-ttu-id="07842-137">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="07842-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="07842-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07842-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers",
    "value": [
        {
            "id": "80b5ddda-1e3b-4c9d-abe2-d606cc075e2e",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com"
        },
        {
            "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com"
        },
        {
            "id": "829e3cb5-3d4d-4319-a8de-1953aedaa166",
            "displayName": "Bob Kelly",
            "emailAddress": "bobk@tailspintoys.com"
        },
        {
            "id": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
            "displayName": "Jordan Miller",
            "emailAddress": "jordanm@contoso.com"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List customers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
