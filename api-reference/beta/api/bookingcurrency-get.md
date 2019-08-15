---
title: Obter bookingCurrency
description: Obtenha as propriedades de um objeto bookingCurrency que está disponível para uma empresa de livros da Microsoft.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b3e6c49ef67d97b636ed29d84a2e085c90305b1f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419437"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="9ac43-103">Obter bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="9ac43-103">Get bookingCurrency</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ac43-104">Obtenha as propriedades de um objeto [bookingCurrency](../resources/bookingcurrency.md) que está disponível para uma empresa de livros da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9ac43-104">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="9ac43-105">Use a propriedade **ID** , que é o código de moeda, para especificar a moeda.</span><span class="sxs-lookup"><span data-stu-id="9ac43-105">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ac43-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ac43-106">Permissions</span></span>
<span data-ttu-id="9ac43-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ac43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ac43-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ac43-109">Permission type</span></span>      | <span data-ttu-id="9ac43-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ac43-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ac43-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ac43-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9ac43-112">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="9ac43-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9ac43-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ac43-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ac43-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ac43-114">Not supported.</span></span>   |
|<span data-ttu-id="9ac43-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ac43-115">Application</span></span> | <span data-ttu-id="9ac43-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ac43-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9ac43-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ac43-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9ac43-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9ac43-118">Optional query parameters</span></span>
<span data-ttu-id="9ac43-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9ac43-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ac43-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ac43-120">Request headers</span></span>
| <span data-ttu-id="9ac43-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9ac43-121">Name</span></span>      |<span data-ttu-id="9ac43-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ac43-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9ac43-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ac43-123">Authorization</span></span>  | <span data-ttu-id="9ac43-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9ac43-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ac43-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ac43-125">Request body</span></span>
<span data-ttu-id="9ac43-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ac43-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9ac43-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ac43-127">Response</span></span>
<span data-ttu-id="9ac43-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingCurrency](../resources/bookingcurrency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ac43-128">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9ac43-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ac43-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ac43-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ac43-130">Request</span></span>
<span data-ttu-id="9ac43-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ac43-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9ac43-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ac43-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ac43-133">C#</span><span class="sxs-lookup"><span data-stu-id="9ac43-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ac43-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ac43-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ac43-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9ac43-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9ac43-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ac43-136">Response</span></span>
<span data-ttu-id="9ac43-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9ac43-137">The following is an example of the response.</span></span> <span data-ttu-id="9ac43-138">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="9ac43-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9ac43-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ac43-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCurrency"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 50

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingCurrencies/$entity",
    "id": "USD",
    "symbol": "$"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingCurrency",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
