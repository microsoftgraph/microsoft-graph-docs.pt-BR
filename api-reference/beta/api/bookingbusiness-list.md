---
title: Lista bookingBusinesses
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 51b8e049b45542de9940168c994bed8fbd273b60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951450"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="e5062-104">Lista bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="e5062-104">List bookingBusinesses</span></span>

 > <span data-ttu-id="e5062-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e5062-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5062-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e5062-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="e5062-107">Obtenha uma coleção de objetos [bookingbusiness](../resources/bookingbusiness.md) que foi criada para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e5062-107">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span> 

<span data-ttu-id="e5062-108">Essa operação retorna apenas a **id** e o **displayName** de cada business reservas na coleção.</span><span class="sxs-lookup"><span data-stu-id="e5062-108">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="e5062-109">Para considerações de desempenho, ele não retorna outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="e5062-109">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="e5062-110">Você pode obter outras propriedades de uma empresa reservas especificando seu **id** em uma operação [obter](bookingbusiness-get.md) .</span><span class="sxs-lookup"><span data-stu-id="e5062-110">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="e5062-111">Você também pode consultar para empresas reservas especificando-se uma cadeia de caracteres em uma `query` parâmetro para subsequência entre as empresas de um inquilino.</span><span class="sxs-lookup"><span data-stu-id="e5062-111">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="e5062-112">Veja um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="e5062-112">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="e5062-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5062-113">Permissions</span></span>
<span data-ttu-id="e5062-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5062-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5062-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5062-116">Permission type</span></span>      | <span data-ttu-id="e5062-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5062-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5062-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5062-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="e5062-119">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="e5062-119">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="e5062-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5062-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5062-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5062-121">Not supported.</span></span>   |
|<span data-ttu-id="e5062-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5062-122">Application</span></span> | <span data-ttu-id="e5062-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5062-123">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="e5062-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5062-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e5062-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e5062-125">Optional query parameters</span></span>
<span data-ttu-id="e5062-126">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e5062-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e5062-127">Este método também oferece suporte a `query` parâmetro que aceita um valor de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="e5062-127">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="e5062-128">Esse parâmetro limita os resultados GET para empresas que coincidem com a cadeia de caracteres especificada.</span><span class="sxs-lookup"><span data-stu-id="e5062-128">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="e5062-129">Você pode ver um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="e5062-129">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="e5062-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5062-130">Request headers</span></span>
| <span data-ttu-id="e5062-131">Nome</span><span class="sxs-lookup"><span data-stu-id="e5062-131">Name</span></span>      |<span data-ttu-id="e5062-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5062-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e5062-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5062-133">Authorization</span></span>  | <span data-ttu-id="e5062-134">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e5062-134">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5062-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5062-135">Request body</span></span>
<span data-ttu-id="e5062-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5062-136">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e5062-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5062-137">Response</span></span>
<span data-ttu-id="e5062-138">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [bookingBusiness](../resources/bookingbusiness.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5062-138">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e5062-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5062-139">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e5062-140">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="e5062-140">Request 1</span></span>
<span data-ttu-id="e5062-141">O exemplo a seguir obtém as empresas reservas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="e5062-141">The following example gets the Bookings businesses in a tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
##### <a name="response-1"></a><span data-ttu-id="e5062-142">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="e5062-142">Response 1</span></span>
<span data-ttu-id="e5062-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5062-143">The following is an example of the response.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="e5062-144">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="e5062-144">Request 2</span></span>
<span data-ttu-id="e5062-145">O exemplo a seguir mostra como usar o `query` parâmetro para obter uma ou mais empresas de reservas correspondentes no inquilino.</span><span class="sxs-lookup"><span data-stu-id="e5062-145">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
##### <a name="response-2"></a><span data-ttu-id="e5062-146">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="e5062-146">Response 2</span></span>
<span data-ttu-id="e5062-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5062-147">The following is an example of the response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List bookingBusinesses",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
