---
title: Listar bookingCurrencies
description: Obtenha uma lista de objetos bookingCurrency disponíveis para uma empresa de livros da Microsoft.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: eb0b9a2e2d122083905c79be7cf540853340d40a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960523"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="545b5-103">Listar bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="545b5-103">List bookingCurrencies</span></span>

<span data-ttu-id="545b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="545b5-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="545b5-105">Obtenha uma lista de objetos [bookingCurrency](../resources/bookingcurrency.md) disponíveis para uma empresa de livros da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="545b5-105">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="545b5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="545b5-106">Permissions</span></span>
<span data-ttu-id="545b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="545b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="545b5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="545b5-109">Permission type</span></span>      | <span data-ttu-id="545b5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="545b5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="545b5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="545b5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="545b5-112">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="545b5-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="545b5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="545b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="545b5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="545b5-114">Not supported.</span></span>   |
|<span data-ttu-id="545b5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="545b5-115">Application</span></span> | <span data-ttu-id="545b5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="545b5-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="545b5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="545b5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="545b5-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="545b5-118">Optional query parameters</span></span>
<span data-ttu-id="545b5-119">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo $count, $filter, $select, $skip e $Top.</span><span class="sxs-lookup"><span data-stu-id="545b5-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="545b5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="545b5-120">Request headers</span></span>
| <span data-ttu-id="545b5-121">Nome</span><span class="sxs-lookup"><span data-stu-id="545b5-121">Name</span></span>      |<span data-ttu-id="545b5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="545b5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="545b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="545b5-123">Authorization</span></span>  | <span data-ttu-id="545b5-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="545b5-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="545b5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="545b5-125">Request body</span></span>
<span data-ttu-id="545b5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="545b5-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="545b5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="545b5-127">Response</span></span>
<span data-ttu-id="545b5-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [bookingCurrency](../resources/bookingcurrency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="545b5-128">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="545b5-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="545b5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="545b5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="545b5-130">Request</span></span>
<span data-ttu-id="545b5-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="545b5-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="545b5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="545b5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingCurrencies
```
# <a name="c"></a>[<span data-ttu-id="545b5-133">C#</span><span class="sxs-lookup"><span data-stu-id="545b5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrencies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="545b5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="545b5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrencies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="545b5-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="545b5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrencies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="545b5-136">Java</span><span class="sxs-lookup"><span data-stu-id="545b5-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingcurrencies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="545b5-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="545b5-137">Response</span></span>
<span data-ttu-id="545b5-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="545b5-138">The following is an example of the response.</span></span> <span data-ttu-id="545b5-139">Observação: o objeto Response mostrado aqui é truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="545b5-139">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="545b5-140">Todas as moedas e propriedades suportadas serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="545b5-140">All of the supported currencies and properties will be returned from an actual call.</span></span>
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
