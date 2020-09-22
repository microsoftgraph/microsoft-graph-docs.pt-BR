---
author: JeremyKelley
ms.author: JeremyKelley
title: Obter listItem
description: Retorna os metadados de um item em uma lista do SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e2d441bb306a6614cdc27f5dff79bd55377b0459
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057281"
---
# <a name="get-listitem"></a><span data-ttu-id="b3294-103">Obter listItem</span><span class="sxs-lookup"><span data-stu-id="b3294-103">Get listItem</span></span>

<span data-ttu-id="b3294-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3294-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3294-105">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="b3294-105">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="b3294-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3294-108">Permissions</span></span>

<span data-ttu-id="b3294-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3294-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3294-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3294-111">Permission type</span></span>      | <span data-ttu-id="b3294-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3294-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3294-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3294-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b3294-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3294-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b3294-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3294-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3294-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3294-116">Not supported.</span></span>    |
|<span data-ttu-id="b3294-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3294-117">Application</span></span> | <span data-ttu-id="b3294-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3294-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3294-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3294-119">HTTP request</span></span>

<span data-ttu-id="b3294-120">Obter um listItem</span><span class="sxs-lookup"><span data-stu-id="b3294-120">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="b3294-121">Obter os valores de coluna de um listItem</span><span class="sxs-lookup"><span data-stu-id="b3294-121">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="b3294-122">Obter valores de coluna específicos de um listItem</span><span class="sxs-lookup"><span data-stu-id="b3294-122">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b3294-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b3294-123">Optional query parameters</span></span>
<span data-ttu-id="b3294-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b3294-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3294-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3294-125">Request headers</span></span>

| <span data-ttu-id="b3294-126">Nome</span><span class="sxs-lookup"><span data-stu-id="b3294-126">Name</span></span>      |<span data-ttu-id="b3294-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3294-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b3294-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3294-128">Authorization</span></span>  | <span data-ttu-id="b3294-129">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="b3294-129">Bearer {code}.</span></span> <span data-ttu-id="b3294-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3294-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3294-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3294-131">Request body</span></span>

<span data-ttu-id="b3294-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3294-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3294-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3294-133">Response</span></span> 

<span data-ttu-id="b3294-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um [item][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3294-134">If successful, this method returns a `200 OK` response code and an [item][] in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3294-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3294-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3294-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3294-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b3294-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3294-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="c"></a>[<span data-ttu-id="b3294-138">C#</span><span class="sxs-lookup"><span data-stu-id="b3294-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3294-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3294-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3294-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3294-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3294-141">Java</span><span class="sxs-lookup"><span data-stu-id="b3294-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b3294-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3294-142">Response</span></span>

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

