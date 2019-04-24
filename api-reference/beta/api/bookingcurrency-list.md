---
title: Listar bookingCurrencies
description: Obtenha uma lista de objetos bookingCurrency disponíveis para uma empresa de livros da Microsoft.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c29ad5780deac5e5e338052c72661f834e483054
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461749"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="7ccbd-103">Listar bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="7ccbd-103">List bookingCurrencies</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ccbd-104">Obtenha uma lista de objetos [bookingCurrency](../resources/bookingcurrency.md) disponíveis para uma empresa de livros da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7ccbd-104">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="7ccbd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ccbd-105">Permissions</span></span>
<span data-ttu-id="7ccbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ccbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ccbd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ccbd-108">Permission type</span></span>      | <span data-ttu-id="7ccbd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ccbd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ccbd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ccbd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7ccbd-111">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="7ccbd-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="7ccbd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ccbd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ccbd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ccbd-113">Not supported.</span></span>   |
|<span data-ttu-id="7ccbd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ccbd-114">Application</span></span> | <span data-ttu-id="7ccbd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ccbd-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7ccbd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ccbd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7ccbd-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7ccbd-117">Optional query parameters</span></span>
<span data-ttu-id="7ccbd-118">Este método oferece suporte aos [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta, incluindo $count, $filter, $select, $skip e $Top.</span><span class="sxs-lookup"><span data-stu-id="7ccbd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ccbd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ccbd-119">Request headers</span></span>
| <span data-ttu-id="7ccbd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7ccbd-120">Name</span></span>      |<span data-ttu-id="7ccbd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ccbd-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7ccbd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ccbd-122">Authorization</span></span>  | <span data-ttu-id="7ccbd-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="7ccbd-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ccbd-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ccbd-124">Request body</span></span>
<span data-ttu-id="7ccbd-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ccbd-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7ccbd-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ccbd-126">Response</span></span>
<span data-ttu-id="7ccbd-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [bookingCurrency](../resources/bookingcurrency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ccbd-127">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7ccbd-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ccbd-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ccbd-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ccbd-129">Request</span></span>
<span data-ttu-id="7ccbd-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ccbd-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a><span data-ttu-id="7ccbd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ccbd-131">Response</span></span>
<span data-ttu-id="7ccbd-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ccbd-132">The following is an example of the response.</span></span> <span data-ttu-id="7ccbd-133">Observação: o objeto Response mostrado aqui é truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="7ccbd-133">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="7ccbd-134">Todas as moedas e propriedades suportadas serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ccbd-134">All of the supported currencies and properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingcurrency-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
