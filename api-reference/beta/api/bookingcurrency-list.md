---
title: Listar bookingCurrencies
description: Obtenha uma lista de objetos bookingCurrency disponíveis para uma empresa de livros da Microsoft.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: cabe3a75518094bcf2fd8e72a46fab955e355571
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419409"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="15e0a-103">Listar bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="15e0a-103">List bookingCurrencies</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15e0a-104">Obtenha uma lista de objetos [bookingCurrency](../resources/bookingcurrency.md) disponíveis para uma empresa de livros da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="15e0a-104">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="15e0a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="15e0a-105">Permissions</span></span>
<span data-ttu-id="15e0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15e0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15e0a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15e0a-108">Permission type</span></span>      | <span data-ttu-id="15e0a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15e0a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15e0a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15e0a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="15e0a-111">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="15e0a-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="15e0a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15e0a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15e0a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15e0a-113">Not supported.</span></span>   |
|<span data-ttu-id="15e0a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15e0a-114">Application</span></span> | <span data-ttu-id="15e0a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15e0a-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="15e0a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15e0a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="15e0a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="15e0a-117">Optional query parameters</span></span>
<span data-ttu-id="15e0a-118">Este método oferece suporte aos [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta, incluindo $count, $filter, $select, $skip e $Top.</span><span class="sxs-lookup"><span data-stu-id="15e0a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15e0a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15e0a-119">Request headers</span></span>
| <span data-ttu-id="15e0a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="15e0a-120">Name</span></span>      |<span data-ttu-id="15e0a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="15e0a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="15e0a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="15e0a-122">Authorization</span></span>  | <span data-ttu-id="15e0a-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="15e0a-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="15e0a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15e0a-124">Request body</span></span>
<span data-ttu-id="15e0a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15e0a-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="15e0a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="15e0a-126">Response</span></span>
<span data-ttu-id="15e0a-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [bookingCurrency](../resources/bookingcurrency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15e0a-127">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="15e0a-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15e0a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15e0a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15e0a-129">Request</span></span>
<span data-ttu-id="15e0a-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="15e0a-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="15e0a-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="15e0a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="15e0a-132">C#</span><span class="sxs-lookup"><span data-stu-id="15e0a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrencies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15e0a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15e0a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrencies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="15e0a-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="15e0a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrencies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="15e0a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="15e0a-135">Response</span></span>
<span data-ttu-id="15e0a-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="15e0a-136">The following is an example of the response.</span></span> <span data-ttu-id="15e0a-137">Observação: o objeto Response mostrado aqui é truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="15e0a-137">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="15e0a-138">Todas as moedas e propriedades suportadas serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15e0a-138">All of the supported currencies and properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCurrency",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingCurrencies",
    "value":[
        {
            "id":"AED",
            "symbol":"د.إ.‏"
        },
        {
            "id":"AFN",
            "symbol":"؋"
        },
        {
            "id":"ALL",
            "symbol":"Lekë"
        },
        {
            "id":"AMD",
            "symbol":"֏"
        },
        {
            "id":"USD",
            "symbol":"$"
        },
        {
            "id":"YER",
            "symbol":"ر.ي.‏"
        },
        {
            "id":"ZAR",
            "symbol":"R"
        },
        {
            "id":"ZMW",
            "symbol":"K"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List bookingCurrencies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
