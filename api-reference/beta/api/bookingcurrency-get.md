---
title: Obter bookingCurrency
description: Obtenha as propriedades de um objeto bookingCurrency que está disponível para uma empresa de livros da Microsoft.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b005f051449538e438ed40b4a89c8355b6cbbace
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720204"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="28ddf-103">Obter bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="28ddf-103">Get bookingCurrency</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28ddf-104">Obtenha as propriedades de um objeto [bookingCurrency](../resources/bookingcurrency.md) que está disponível para uma empresa de livros da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="28ddf-104">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="28ddf-105">Use a propriedade **ID** , que é o código de moeda, para especificar a moeda.</span><span class="sxs-lookup"><span data-stu-id="28ddf-105">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="28ddf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="28ddf-106">Permissions</span></span>
<span data-ttu-id="28ddf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28ddf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28ddf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28ddf-109">Permission type</span></span>      | <span data-ttu-id="28ddf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28ddf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28ddf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28ddf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="28ddf-112">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="28ddf-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="28ddf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28ddf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28ddf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28ddf-114">Not supported.</span></span>   |
|<span data-ttu-id="28ddf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28ddf-115">Application</span></span> | <span data-ttu-id="28ddf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28ddf-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="28ddf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28ddf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="28ddf-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="28ddf-118">Optional query parameters</span></span>
<span data-ttu-id="28ddf-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="28ddf-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28ddf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28ddf-120">Request headers</span></span>
| <span data-ttu-id="28ddf-121">Nome</span><span class="sxs-lookup"><span data-stu-id="28ddf-121">Name</span></span>      |<span data-ttu-id="28ddf-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="28ddf-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="28ddf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="28ddf-123">Authorization</span></span>  | <span data-ttu-id="28ddf-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="28ddf-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="28ddf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28ddf-125">Request body</span></span>
<span data-ttu-id="28ddf-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28ddf-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="28ddf-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="28ddf-127">Response</span></span>
<span data-ttu-id="28ddf-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingCurrency](../resources/bookingcurrency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28ddf-128">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="28ddf-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28ddf-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28ddf-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28ddf-130">Request</span></span>
<span data-ttu-id="28ddf-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="28ddf-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="28ddf-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="28ddf-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="28ddf-133">C#</span><span class="sxs-lookup"><span data-stu-id="28ddf-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28ddf-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28ddf-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="28ddf-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="28ddf-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28ddf-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="28ddf-136">Response</span></span>
<span data-ttu-id="28ddf-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="28ddf-137">The following is an example of the response.</span></span> <span data-ttu-id="28ddf-138">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="28ddf-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="28ddf-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28ddf-139">All of the properties will be returned from an actual call.</span></span>
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
