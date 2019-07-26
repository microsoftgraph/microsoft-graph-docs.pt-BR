---
author: JeremyKelley
ms.author: JeremyKelley
title: Obter listItem
description: Retorna os metadados de um item em uma lista do SharePoint.
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 5046cbc44b80f6306c9e948bfbb8fce8427da117
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880696"
---
# <a name="get-listitem"></a><span data-ttu-id="d1d3b-103">Obter listItem</span><span class="sxs-lookup"><span data-stu-id="d1d3b-103">Get listItem</span></span>

<span data-ttu-id="d1d3b-104">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="d1d3b-104">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="d1d3b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1d3b-107">Permissions</span></span>

<span data-ttu-id="d1d3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1d3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1d3b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1d3b-110">Permission type</span></span>      | <span data-ttu-id="d1d3b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1d3b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1d3b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1d3b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d1d3b-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1d3b-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d1d3b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1d3b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1d3b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1d3b-115">Not supported.</span></span>    |
|<span data-ttu-id="d1d3b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1d3b-116">Application</span></span> | <span data-ttu-id="d1d3b-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1d3b-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1d3b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1d3b-118">HTTP request</span></span>

<span data-ttu-id="d1d3b-119">Obter um listItem</span><span class="sxs-lookup"><span data-stu-id="d1d3b-119">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="d1d3b-120">Obter os valores de coluna de um listItem</span><span class="sxs-lookup"><span data-stu-id="d1d3b-120">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="d1d3b-121">Obter valores de coluna específicos de um listItem</span><span class="sxs-lookup"><span data-stu-id="d1d3b-121">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d1d3b-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1d3b-122">Optional query parameters</span></span>
<span data-ttu-id="d1d3b-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d1d3b-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1d3b-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1d3b-124">Request headers</span></span>

| <span data-ttu-id="d1d3b-125">Nome</span><span class="sxs-lookup"><span data-stu-id="d1d3b-125">Name</span></span>      |<span data-ttu-id="d1d3b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1d3b-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d1d3b-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1d3b-127">Authorization</span></span>  | <span data-ttu-id="d1d3b-128">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="d1d3b-128">Bearer {code}.</span></span> <span data-ttu-id="d1d3b-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1d3b-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1d3b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1d3b-130">Request body</span></span>

<span data-ttu-id="d1d3b-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1d3b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1d3b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1d3b-132">Response</span></span> 

<span data-ttu-id="d1d3b-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um [item][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1d3b-133">If successful, this method returns a `200 OK` response code and an [item][] in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1d3b-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1d3b-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1d3b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1d3b-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d1d3b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1d3b-136">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d1d3b-137">C#</span><span class="sxs-lookup"><span data-stu-id="d1d3b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1d3b-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="d1d3b-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d1d3b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1d3b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d1d3b-140">Java</span><span class="sxs-lookup"><span data-stu-id="d1d3b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d1d3b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1d3b-141">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "5",
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
  ]
} -->
