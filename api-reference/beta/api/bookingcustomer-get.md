---
title: Obter bookingCustomer
description: Obtenha as propriedades e os relacionamentos de um objeto bookingCustomer.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b3091f9e2fa869640609faefb8f0a4d326068602
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35257894"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="52ebd-103">Obter bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="52ebd-103">Get bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52ebd-104">Obtenha as propriedades e os relacionamentos de um objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="52ebd-104">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="52ebd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="52ebd-105">Permissions</span></span>
<span data-ttu-id="52ebd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52ebd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52ebd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52ebd-108">Permission type</span></span>      | <span data-ttu-id="52ebd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52ebd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52ebd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52ebd-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="52ebd-111">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="52ebd-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="52ebd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52ebd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52ebd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52ebd-113">Not supported.</span></span>   |
|<span data-ttu-id="52ebd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52ebd-114">Application</span></span> | <span data-ttu-id="52ebd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52ebd-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="52ebd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52ebd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="52ebd-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="52ebd-117">Optional query parameters</span></span>
<span data-ttu-id="52ebd-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="52ebd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52ebd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52ebd-119">Request headers</span></span>
| <span data-ttu-id="52ebd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="52ebd-120">Name</span></span>      |<span data-ttu-id="52ebd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="52ebd-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="52ebd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="52ebd-122">Authorization</span></span>  | <span data-ttu-id="52ebd-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="52ebd-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="52ebd-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52ebd-124">Request body</span></span>
<span data-ttu-id="52ebd-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52ebd-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="52ebd-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="52ebd-126">Response</span></span>
<span data-ttu-id="52ebd-127">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingCustomer](../resources/bookingcustomer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52ebd-127">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="52ebd-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52ebd-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52ebd-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52ebd-129">Request</span></span>
<span data-ttu-id="52ebd-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52ebd-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
##### <a name="response"></a><span data-ttu-id="52ebd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="52ebd-131">Response</span></span>
<span data-ttu-id="52ebd-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52ebd-132">The following is an example of the response.</span></span> <span data-ttu-id="52ebd-133">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="52ebd-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="52ebd-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52ebd-134">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="52ebd-135">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="52ebd-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="52ebd-136">C#</span><span class="sxs-lookup"><span data-stu-id="52ebd-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingcustomer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52ebd-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="52ebd-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingcustomer-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="52ebd-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="52ebd-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_bookingcustomer-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingcustomer-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingcustomer-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingcustomer-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
