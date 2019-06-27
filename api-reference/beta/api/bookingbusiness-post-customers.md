---
title: Criar bookingCustomer
description: Criar um novo objeto bookingCustomer.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a7ad80e8caf0e8c38479fc58dc7b677c58617770
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258153"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="de3e4-103">Criar bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="de3e4-103">Create bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de3e4-104">Criar um novo objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="de3e4-104">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="de3e4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="de3e4-105">Permissions</span></span>
<span data-ttu-id="de3e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de3e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de3e4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de3e4-108">Permission type</span></span>      | <span data-ttu-id="de3e4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de3e4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de3e4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de3e4-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="de3e4-111">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="de3e4-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="de3e4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de3e4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de3e4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de3e4-113">Not supported.</span></span>   |
|<span data-ttu-id="de3e4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de3e4-114">Application</span></span> | <span data-ttu-id="de3e4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de3e4-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="de3e4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de3e4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="de3e4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de3e4-117">Request headers</span></span>
| <span data-ttu-id="de3e4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="de3e4-118">Name</span></span>       | <span data-ttu-id="de3e4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="de3e4-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="de3e4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="de3e4-120">Authorization</span></span>  | <span data-ttu-id="de3e4-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="de3e4-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="de3e4-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de3e4-122">Request body</span></span>
<span data-ttu-id="de3e4-123">No corpo da solicitação, forneça uma representação JSON do objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="de3e4-123">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="de3e4-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="de3e4-124">Response</span></span>
<span data-ttu-id="de3e4-125">Se bem-sucedido, este método retorna `201, Created` o código de resposta e o objeto [bookingCustomer](../resources/bookingcustomer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de3e4-125">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de3e4-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de3e4-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de3e4-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de3e4-127">Request</span></span>
<span data-ttu-id="de3e4-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="de3e4-128">The following is an example of the request.</span></span>
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
<span data-ttu-id="de3e4-129">No corpo da solicitação, forneça uma representação JSON do objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="de3e4-129">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="de3e4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="de3e4-130">Response</span></span>
<span data-ttu-id="de3e4-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="de3e4-131">The following is an example of the response.</span></span> <span data-ttu-id="de3e4-132">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="de3e4-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="de3e4-133">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de3e4-133">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="de3e4-134">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="de3e4-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="de3e4-135">C#</span><span class="sxs-lookup"><span data-stu-id="de3e4-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_bookingcustomer_from_bookingbusiness-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de3e4-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="de3e4-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_bookingcustomer_from_bookingbusiness-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="de3e4-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="de3e4-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_bookingcustomer_from_bookingbusiness-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-post-customers.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-post-customers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-post-customers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
