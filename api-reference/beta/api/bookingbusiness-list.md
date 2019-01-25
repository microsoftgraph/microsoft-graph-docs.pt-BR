---
title: Lista bookingBusinesses
description: Obtenha uma coleção de objetos bookingbusiness que foi criada para o inquilino.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 8018b8ac7f9d2e5f74e4233dbc36c2a6faa2d9a8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523152"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="b8e7c-103">Lista bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="b8e7c-103">List bookingBusinesses</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8e7c-104">Obtenha uma coleção de objetos [bookingbusiness](../resources/bookingbusiness.md) que foi criada para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-104">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span>

<span data-ttu-id="b8e7c-105">Essa operação retorna apenas a **id** e o **displayName** de cada business reservas na coleção.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-105">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="b8e7c-106">Para considerações de desempenho, ele não retorna outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-106">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="b8e7c-107">Você pode obter outras propriedades de uma empresa reservas especificando seu **id** em uma operação [obter](bookingbusiness-get.md) .</span><span class="sxs-lookup"><span data-stu-id="b8e7c-107">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="b8e7c-108">Você também pode consultar para empresas reservas especificando-se uma cadeia de caracteres em uma `query` parâmetro para subsequência entre as empresas de um inquilino.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-108">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="b8e7c-109">Veja um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-109">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="b8e7c-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8e7c-110">Permissions</span></span>
<span data-ttu-id="b8e7c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8e7c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8e7c-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8e7c-113">Permission type</span></span>      | <span data-ttu-id="b8e7c-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8e7c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8e7c-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8e7c-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="b8e7c-116">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="b8e7c-116">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b8e7c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8e7c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8e7c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-118">Not supported.</span></span>   |
|<span data-ttu-id="b8e7c-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8e7c-119">Application</span></span> | <span data-ttu-id="b8e7c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-120">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="b8e7c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8e7c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b8e7c-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b8e7c-122">Optional query parameters</span></span>
<span data-ttu-id="b8e7c-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b8e7c-124">Este método também oferece suporte a `query` parâmetro que aceita um valor de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-124">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="b8e7c-125">Esse parâmetro limita os resultados GET para empresas que coincidem com a cadeia de caracteres especificada.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-125">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="b8e7c-126">Você pode ver um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-126">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="b8e7c-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8e7c-127">Request headers</span></span>
| <span data-ttu-id="b8e7c-128">Nome</span><span class="sxs-lookup"><span data-stu-id="b8e7c-128">Name</span></span>      |<span data-ttu-id="b8e7c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8e7c-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b8e7c-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8e7c-130">Authorization</span></span>  | <span data-ttu-id="b8e7c-131">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="b8e7c-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8e7c-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8e7c-132">Request body</span></span>
<span data-ttu-id="b8e7c-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b8e7c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8e7c-134">Response</span></span>
<span data-ttu-id="b8e7c-135">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [bookingBusiness](../resources/bookingbusiness.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-135">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b8e7c-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8e7c-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="b8e7c-137">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="b8e7c-137">Request 1</span></span>
<span data-ttu-id="b8e7c-138">O exemplo a seguir obtém as empresas reservas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-138">The following example gets the Bookings businesses in a tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
##### <a name="response-1"></a><span data-ttu-id="b8e7c-139">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="b8e7c-139">Response 1</span></span>
<span data-ttu-id="b8e7c-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-140">The following is an example of the response.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="b8e7c-141">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="b8e7c-141">Request 2</span></span>
<span data-ttu-id="b8e7c-142">O exemplo a seguir mostra como usar o `query` parâmetro para obter uma ou mais empresas de reservas correspondentes no inquilino.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-142">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
##### <a name="response-2"></a><span data-ttu-id="b8e7c-143">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="b8e7c-143">Response 2</span></span>
<span data-ttu-id="b8e7c-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8e7c-144">The following is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
