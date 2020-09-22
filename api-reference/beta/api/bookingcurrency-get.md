---
title: Obter bookingCurrency
description: Obtenha as propriedades de um objeto bookingCurrency que está disponível para uma empresa de livros da Microsoft.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 31d8791f6ae2345bedffa7fe25a80f83651bda3e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987950"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="d3a73-103">Obter bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="d3a73-103">Get bookingCurrency</span></span>

<span data-ttu-id="d3a73-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3a73-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3a73-105">Obtenha as propriedades de um objeto [bookingCurrency](../resources/bookingcurrency.md) que está disponível para uma empresa de livros da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d3a73-105">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="d3a73-106">Use a propriedade **ID** , que é o código de moeda, para especificar a moeda.</span><span class="sxs-lookup"><span data-stu-id="d3a73-106">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3a73-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3a73-107">Permissions</span></span>
<span data-ttu-id="d3a73-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3a73-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3a73-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3a73-110">Permission type</span></span>      | <span data-ttu-id="d3a73-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3a73-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3a73-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3a73-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d3a73-113">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="d3a73-113">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d3a73-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3a73-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3a73-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3a73-115">Not supported.</span></span>   |
|<span data-ttu-id="d3a73-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3a73-116">Application</span></span> | <span data-ttu-id="d3a73-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3a73-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d3a73-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3a73-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d3a73-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d3a73-119">Optional query parameters</span></span>
<span data-ttu-id="d3a73-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d3a73-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3a73-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a73-121">Request headers</span></span>
| <span data-ttu-id="d3a73-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d3a73-122">Name</span></span>      |<span data-ttu-id="d3a73-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3a73-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d3a73-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3a73-124">Authorization</span></span>  | <span data-ttu-id="d3a73-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d3a73-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3a73-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a73-126">Request body</span></span>
<span data-ttu-id="d3a73-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3a73-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d3a73-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3a73-128">Response</span></span>
<span data-ttu-id="d3a73-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingCurrency](../resources/bookingcurrency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3a73-129">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d3a73-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3a73-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3a73-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a73-131">Request</span></span>
<span data-ttu-id="d3a73-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3a73-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3a73-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3a73-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
# <a name="c"></a>[<span data-ttu-id="d3a73-134">C#</span><span class="sxs-lookup"><span data-stu-id="d3a73-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3a73-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3a73-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3a73-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3a73-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d3a73-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3a73-137">Response</span></span>
<span data-ttu-id="d3a73-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d3a73-138">The following is an example of the response.</span></span> <span data-ttu-id="d3a73-139">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="d3a73-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d3a73-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3a73-140">All of the properties will be returned from an actual call.</span></span>
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


