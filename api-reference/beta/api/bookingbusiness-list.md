---
title: Listar bookingBusinesses
description: Obtenha uma coleção de objetos bookingbusiness que foi criada para o locatário.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: c1cf4042fbfbbc3364756c9363555215bff05e01
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960767"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="9d2e1-103">Listar bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="9d2e1-103">List bookingBusinesses</span></span>

<span data-ttu-id="9d2e1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d2e1-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d2e1-105">Obtenha uma coleção de objetos [bookingbusiness](../resources/bookingbusiness.md) que foi criada para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-105">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span>

<span data-ttu-id="9d2e1-106">Essa operação retorna apenas a **ID** e o **DisplayName** de cada livro de livros na coleção.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-106">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="9d2e1-107">Para considerações de desempenho, ele não retorna outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-107">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="9d2e1-108">Você pode obter as outras propriedades de uma empresa de livros, especificando sua **ID** em uma operação [Get](bookingbusiness-get.md) .</span><span class="sxs-lookup"><span data-stu-id="9d2e1-108">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="9d2e1-109">Você também pode consultar as empresas de reservas especificando uma cadeia de caracteres em um `query` parâmetro para fazer a correspondência de subcadeia entre as empresas de um locatário.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-109">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="9d2e1-110">Veja um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-110">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="9d2e1-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d2e1-111">Permissions</span></span>
<span data-ttu-id="9d2e1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d2e1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d2e1-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d2e1-114">Permission type</span></span>      | <span data-ttu-id="9d2e1-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9d2e1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d2e1-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d2e1-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="9d2e1-117">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="9d2e1-117">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9d2e1-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d2e1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d2e1-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-119">Not supported.</span></span>   |
|<span data-ttu-id="9d2e1-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d2e1-120">Application</span></span> | <span data-ttu-id="9d2e1-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9d2e1-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d2e1-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9d2e1-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9d2e1-123">Optional query parameters</span></span>
<span data-ttu-id="9d2e1-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="9d2e1-125">Este método também dá suporte ao `query` parâmetro que aceita um valor de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-125">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="9d2e1-126">Esse parâmetro limita os resultados GET para empresas que correspondem à cadeia de caracteres especificada.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-126">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="9d2e1-127">Você pode ver um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-127">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="9d2e1-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d2e1-128">Request headers</span></span>
| <span data-ttu-id="9d2e1-129">Nome</span><span class="sxs-lookup"><span data-stu-id="9d2e1-129">Name</span></span>      |<span data-ttu-id="9d2e1-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d2e1-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9d2e1-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d2e1-131">Authorization</span></span>  | <span data-ttu-id="9d2e1-132">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9d2e1-132">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d2e1-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d2e1-133">Request body</span></span>
<span data-ttu-id="9d2e1-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-134">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9d2e1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d2e1-135">Response</span></span>
<span data-ttu-id="9d2e1-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [bookingBusiness](../resources/bookingbusiness.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-136">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9d2e1-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d2e1-137">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="9d2e1-138">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="9d2e1-138">Request 1</span></span>
<span data-ttu-id="9d2e1-139">O exemplo a seguir obtém as empresas de reservas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-139">The following example gets the Bookings businesses in a tenant.</span></span>

# <a name="http"></a>[<span data-ttu-id="9d2e1-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d2e1-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses
```
# <a name="c"></a>[<span data-ttu-id="9d2e1-141">C#</span><span class="sxs-lookup"><span data-stu-id="9d2e1-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingbusinesses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d2e1-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d2e1-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingbusinesses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d2e1-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d2e1-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingbusinesses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d2e1-144">Java</span><span class="sxs-lookup"><span data-stu-id="9d2e1-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingbusinesses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="9d2e1-145">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="9d2e1-145">Response 1</span></span>
<span data-ttu-id="9d2e1-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-146">The following is an example of the response.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="9d2e1-147">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="9d2e1-147">Request 2</span></span>
<span data-ttu-id="9d2e1-148">O exemplo a seguir mostra como usar o `query` parâmetro para obter uma ou mais empresas de reservas correspondentes no locatário.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-148">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>

# <a name="http"></a>[<span data-ttu-id="9d2e1-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d2e1-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
# <a name="c"></a>[<span data-ttu-id="9d2e1-150">C#</span><span class="sxs-lookup"><span data-stu-id="9d2e1-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/query-bookingbusinesses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d2e1-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d2e1-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/query-bookingbusinesses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d2e1-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d2e1-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/query-bookingbusinesses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d2e1-153">Java</span><span class="sxs-lookup"><span data-stu-id="9d2e1-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/query-bookingbusinesses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="9d2e1-154">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="9d2e1-154">Response 2</span></span>
<span data-ttu-id="9d2e1-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9d2e1-155">The following is an example of the response.</span></span>
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
