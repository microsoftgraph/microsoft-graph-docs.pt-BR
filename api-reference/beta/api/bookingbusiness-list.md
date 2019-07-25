---
title: Listar bookingBusinesses
description: Obtenha uma coleção de objetos bookingbusiness que foi criada para o locatário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 1dfea8576e8177478a3e21e326bc8dd7402cacfb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865631"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="d90c9-103">Listar bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="d90c9-103">List bookingBusinesses</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d90c9-104">Obtenha uma coleção de objetos [bookingbusiness](../resources/bookingbusiness.md) que foi criada para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d90c9-104">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span>

<span data-ttu-id="d90c9-105">Essa operação retorna apenas a **ID** e o **DisplayName** de cada livro de livros na coleção.</span><span class="sxs-lookup"><span data-stu-id="d90c9-105">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="d90c9-106">Para considerações de desempenho, ele não retorna outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="d90c9-106">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="d90c9-107">Você pode obter as outras propriedades de uma empresa de livros, especificando sua **ID** em uma operação [Get](bookingbusiness-get.md) .</span><span class="sxs-lookup"><span data-stu-id="d90c9-107">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="d90c9-108">Você também pode consultar as empresas de reservas especificando uma cadeia de caracteres em `query` um parâmetro para fazer a correspondência de subcadeia entre as empresas de um locatário.</span><span class="sxs-lookup"><span data-stu-id="d90c9-108">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="d90c9-109">Veja um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="d90c9-109">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="d90c9-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d90c9-110">Permissions</span></span>
<span data-ttu-id="d90c9-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d90c9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d90c9-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d90c9-113">Permission type</span></span>      | <span data-ttu-id="d90c9-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d90c9-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d90c9-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d90c9-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="d90c9-116">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="d90c9-116">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d90c9-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d90c9-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d90c9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d90c9-118">Not supported.</span></span>   |
|<span data-ttu-id="d90c9-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d90c9-119">Application</span></span> | <span data-ttu-id="d90c9-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d90c9-120">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d90c9-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d90c9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d90c9-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d90c9-122">Optional query parameters</span></span>
<span data-ttu-id="d90c9-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d90c9-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d90c9-124">Este método também dá suporte `query` ao parâmetro que aceita um valor de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="d90c9-124">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="d90c9-125">Esse parâmetro limita os resultados GET para empresas que correspondem à cadeia de caracteres especificada.</span><span class="sxs-lookup"><span data-stu-id="d90c9-125">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="d90c9-126">Você pode ver um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="d90c9-126">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="d90c9-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d90c9-127">Request headers</span></span>
| <span data-ttu-id="d90c9-128">Nome</span><span class="sxs-lookup"><span data-stu-id="d90c9-128">Name</span></span>      |<span data-ttu-id="d90c9-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="d90c9-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d90c9-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="d90c9-130">Authorization</span></span>  | <span data-ttu-id="d90c9-131">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d90c9-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d90c9-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d90c9-132">Request body</span></span>
<span data-ttu-id="d90c9-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d90c9-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d90c9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d90c9-134">Response</span></span>
<span data-ttu-id="d90c9-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [bookingBusiness](../resources/bookingbusiness.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d90c9-135">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d90c9-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d90c9-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="d90c9-137">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="d90c9-137">Request 1</span></span>
<span data-ttu-id="d90c9-138">O exemplo a seguir obtém as empresas de reservas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="d90c9-138">The following example gets the Bookings businesses in a tenant.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d90c9-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="d90c9-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d90c9-140">C#</span><span class="sxs-lookup"><span data-stu-id="d90c9-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingbusinesses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d90c9-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="d90c9-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingbusinesses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d90c9-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d90c9-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingbusinesses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d90c9-143">Java</span><span class="sxs-lookup"><span data-stu-id="d90c9-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingbusinesses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="d90c9-144">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="d90c9-144">Response 1</span></span>
<span data-ttu-id="d90c9-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d90c9-145">The following is an example of the response.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="d90c9-146">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="d90c9-146">Request 2</span></span>
<span data-ttu-id="d90c9-147">O exemplo a seguir mostra como usar o `query` parâmetro para obter uma ou mais empresas de reservas correspondentes no locatário.</span><span class="sxs-lookup"><span data-stu-id="d90c9-147">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d90c9-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="d90c9-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d90c9-149">C#</span><span class="sxs-lookup"><span data-stu-id="d90c9-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/query-bookingbusinesses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d90c9-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="d90c9-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/query-bookingbusinesses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d90c9-151">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d90c9-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/query-bookingbusinesses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d90c9-152">Java</span><span class="sxs-lookup"><span data-stu-id="d90c9-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/query-bookingbusinesses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="d90c9-153">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="d90c9-153">Response 2</span></span>
<span data-ttu-id="d90c9-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d90c9-154">The following is an example of the response.</span></span>
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
  ]
}
-->
