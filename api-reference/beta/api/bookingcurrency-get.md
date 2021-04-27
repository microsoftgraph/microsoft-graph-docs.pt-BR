---
title: Obter bookingCurrency
description: Obter as propriedades de um objeto bookingCurrency que está disponível para uma empresa do Microsoft Bookings.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: f6702d108c3b705749021ad79d7e9fe6ceb944b1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047837"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="1a6ff-103">Obter bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="1a6ff-103">Get bookingCurrency</span></span>

<span data-ttu-id="1a6ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a6ff-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a6ff-105">Obter as propriedades de um [objeto bookingCurrency](../resources/bookingcurrency.md) que está disponível para uma empresa do Microsoft Bookings.</span><span class="sxs-lookup"><span data-stu-id="1a6ff-105">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="1a6ff-106">Use a **propriedade id,** que é o código de moeda, para especificar a moeda.</span><span class="sxs-lookup"><span data-stu-id="1a6ff-106">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a6ff-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a6ff-107">Permissions</span></span>
<span data-ttu-id="1a6ff-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a6ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a6ff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a6ff-110">Permission type</span></span>      | <span data-ttu-id="1a6ff-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a6ff-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a6ff-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a6ff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1a6ff-113">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="1a6ff-113">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1a6ff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a6ff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a6ff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a6ff-115">Not supported.</span></span>   |
|<span data-ttu-id="1a6ff-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a6ff-116">Application</span></span> | <span data-ttu-id="1a6ff-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a6ff-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1a6ff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a6ff-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1a6ff-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1a6ff-119">Optional query parameters</span></span>
<span data-ttu-id="1a6ff-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1a6ff-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a6ff-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a6ff-121">Request headers</span></span>
| <span data-ttu-id="1a6ff-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1a6ff-122">Name</span></span>      |<span data-ttu-id="1a6ff-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a6ff-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1a6ff-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a6ff-124">Authorization</span></span>  | <span data-ttu-id="1a6ff-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="1a6ff-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a6ff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a6ff-126">Request body</span></span>
<span data-ttu-id="1a6ff-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1a6ff-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1a6ff-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a6ff-128">Response</span></span>
<span data-ttu-id="1a6ff-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto bookingCurrency](../resources/bookingcurrency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a6ff-129">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a6ff-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a6ff-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a6ff-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a6ff-131">Request</span></span>
<span data-ttu-id="1a6ff-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a6ff-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a6ff-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a6ff-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
# <a name="c"></a>[<span data-ttu-id="1a6ff-134">C#</span><span class="sxs-lookup"><span data-stu-id="1a6ff-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a6ff-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a6ff-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a6ff-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a6ff-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a6ff-137">Java</span><span class="sxs-lookup"><span data-stu-id="1a6ff-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingcurrency-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1a6ff-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a6ff-138">Response</span></span>
<span data-ttu-id="1a6ff-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1a6ff-139">The following is an example of the response.</span></span> <span data-ttu-id="1a6ff-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1a6ff-140">Note: The response object shown here might be shortened for readability.</span></span>
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
