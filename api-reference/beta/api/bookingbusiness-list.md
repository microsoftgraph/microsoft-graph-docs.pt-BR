---
title: Listar bookingBusinesses
description: Obtenha uma coleção de objetos bookingbusiness que foi criada para o locatário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: ef7581d9e87cdc2e367fe557fbc9a15b018c78c6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258104"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="d3797-103">Listar bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="d3797-103">List bookingBusinesses</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3797-104">Obtenha uma coleção de objetos [bookingbusiness](../resources/bookingbusiness.md) que foi criada para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3797-104">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span>

<span data-ttu-id="d3797-105">Essa operação retorna apenas a **ID** e o **DisplayName** de cada livro de livros na coleção.</span><span class="sxs-lookup"><span data-stu-id="d3797-105">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="d3797-106">Para considerações de desempenho, ele não retorna outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="d3797-106">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="d3797-107">Você pode obter as outras propriedades de uma empresa de livros, especificando sua **ID** em uma operação [Get](bookingbusiness-get.md) .</span><span class="sxs-lookup"><span data-stu-id="d3797-107">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="d3797-108">Você também pode consultar as empresas de reservas especificando uma cadeia de caracteres em `query` um parâmetro para fazer a correspondência de subcadeia entre as empresas de um locatário.</span><span class="sxs-lookup"><span data-stu-id="d3797-108">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="d3797-109">Veja um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="d3797-109">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="d3797-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3797-110">Permissions</span></span>
<span data-ttu-id="d3797-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3797-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3797-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3797-113">Permission type</span></span>      | <span data-ttu-id="d3797-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3797-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3797-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3797-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="d3797-116">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="d3797-116">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d3797-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3797-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3797-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3797-118">Not supported.</span></span>   |
|<span data-ttu-id="d3797-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3797-119">Application</span></span> | <span data-ttu-id="d3797-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3797-120">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d3797-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3797-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d3797-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d3797-122">Optional query parameters</span></span>
<span data-ttu-id="d3797-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d3797-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d3797-124">Este método também dá suporte `query` ao parâmetro que aceita um valor de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="d3797-124">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="d3797-125">Esse parâmetro limita os resultados GET para empresas que correspondem à cadeia de caracteres especificada.</span><span class="sxs-lookup"><span data-stu-id="d3797-125">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="d3797-126">Você pode ver um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="d3797-126">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="d3797-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3797-127">Request headers</span></span>
| <span data-ttu-id="d3797-128">Nome</span><span class="sxs-lookup"><span data-stu-id="d3797-128">Name</span></span>      |<span data-ttu-id="d3797-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3797-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d3797-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3797-130">Authorization</span></span>  | <span data-ttu-id="d3797-131">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d3797-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3797-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3797-132">Request body</span></span>
<span data-ttu-id="d3797-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3797-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d3797-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3797-134">Response</span></span>
<span data-ttu-id="d3797-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [bookingBusiness](../resources/bookingbusiness.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3797-135">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d3797-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3797-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="d3797-137">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="d3797-137">Request 1</span></span>
<span data-ttu-id="d3797-138">O exemplo a seguir obtém as empresas de reservas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="d3797-138">The following example gets the Bookings businesses in a tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
##### <a name="response-1"></a><span data-ttu-id="d3797-139">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="d3797-139">Response 1</span></span>
<span data-ttu-id="d3797-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d3797-140">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"Contosolunchdelivery@M365B489948.onmicrosoft.com",
            "displayName":"Contoso lunch delivery",
        },
        {
            "id":"Fabrikam@M365B489948.onmicrosoft.com",
            "displayName":"Fabrikam",
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3797-141">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="d3797-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3797-142">C#</span><span class="sxs-lookup"><span data-stu-id="d3797-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingbusinesses-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3797-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3797-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingbusinesses-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d3797-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d3797-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_bookingbusinesses-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


##### <a name="request-2"></a><span data-ttu-id="d3797-145">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="d3797-145">Request 2</span></span>
<span data-ttu-id="d3797-146">O exemplo a seguir mostra como usar o `query` parâmetro para obter uma ou mais empresas de reservas correspondentes no locatário.</span><span class="sxs-lookup"><span data-stu-id="d3797-146">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
##### <a name="response-2"></a><span data-ttu-id="d3797-147">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="d3797-147">Response 2</span></span>
<span data-ttu-id="d3797-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d3797-148">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"AdventureWorksCycles@M365B960066.onmicrosoft.com",
            "displayName":"Adventure Works Cycles",
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3797-149">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="d3797-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3797-150">C#</span><span class="sxs-lookup"><span data-stu-id="d3797-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/query_bookingbusinesses-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3797-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3797-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/query_bookingbusinesses-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d3797-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d3797-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/query_bookingbusinesses-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List bookingBusinesses",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
