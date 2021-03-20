---
author: swapnil1993
title: 'contentType: addCopy'
description: Adicione uma cópia de um tipo de conteúdo de site a uma lista.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: f388799e409a5f2037182bb3bc331a6a6adbc45f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947025"
---
# <a name="contenttype-addcopy"></a><span data-ttu-id="6d520-103">contentType: addCopy</span><span class="sxs-lookup"><span data-stu-id="6d520-103">contentType: addCopy</span></span>
<span data-ttu-id="6d520-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d520-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="6d520-105">Adicione uma cópia de um [tipo de conteúdo][contentType] de um [site][site] a uma [lista][list].</span><span class="sxs-lookup"><span data-stu-id="6d520-105">Add a copy of a [content type][contentType] from a [site][site] to a [list][list].</span></span>
 
  

## <a name="permissions"></a><span data-ttu-id="6d520-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d520-106">Permissions</span></span>  

<span data-ttu-id="6d520-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6d520-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="6d520-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d520-109">Permission type</span></span> | <span data-ttu-id="6d520-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d520-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d520-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d520-111">Delegated (work or school account)</span></span> |<span data-ttu-id="6d520-112">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6d520-112">Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="6d520-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d520-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d520-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d520-114">Not supported.</span></span> |
|<span data-ttu-id="6d520-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d520-115">Application</span></span> | <span data-ttu-id="6d520-116">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6d520-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="6d520-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d520-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/{site-id}/lists/{list-id}/contentTypes/addCopy
```

## <a name="request-headers"></a><span data-ttu-id="6d520-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d520-118">Request headers</span></span>
|<span data-ttu-id="6d520-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6d520-119">Name</span></span>|<span data-ttu-id="6d520-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d520-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6d520-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d520-121">Authorization</span></span>|<span data-ttu-id="6d520-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d520-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6d520-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d520-124">Content-Type</span></span>|<span data-ttu-id="6d520-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d520-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d520-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d520-127">Request body</span></span>
<span data-ttu-id="6d520-128">No corpo da solicitação, fornece uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="6d520-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="6d520-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="6d520-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6d520-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6d520-130">Parameter</span></span>|<span data-ttu-id="6d520-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d520-131">Type</span></span>|<span data-ttu-id="6d520-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d520-132">Description</span></span>|
|-|-|-|
|<span data-ttu-id="6d520-133">contentType</span><span class="sxs-lookup"><span data-stu-id="6d520-133">contentType</span></span>| <span data-ttu-id="6d520-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d520-134">string</span></span> | <span data-ttu-id="6d520-135">URL canônica para o tipo de conteúdo do site que será copiado para a lista.</span><span class="sxs-lookup"><span data-stu-id="6d520-135">Canonical URL to the site content type that will be copied to the list.</span></span> <span data-ttu-id="6d520-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d520-136">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="6d520-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d520-137">Response</span></span>

<span data-ttu-id="6d520-138">Se tiver êxito, essa chamada retornará um código `201 Created` de resposta e um objeto [contentType][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d520-138">If successful, this call returns a `201 Created` response code and a [contentType][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d520-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d520-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d520-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d520-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6d520-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d520-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_addcopy"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/id/lists/{list-id}/contentTypes/addCopy
Content-Type: application/json

{
  "contentType": "https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101"
}
```
# <a name="c"></a>[<span data-ttu-id="6d520-142">C#</span><span class="sxs-lookup"><span data-stu-id="6d520-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-addcopy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d520-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d520-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-addcopy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d520-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d520-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-addcopy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6d520-145">Java</span><span class="sxs-lookup"><span data-stu-id="6d520-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-addcopy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a><span data-ttu-id="6d520-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d520-146">Response</span></span>


<!-- { "blockType": "response", "@type": "microsoft.graph.contentType", "truncated": true} -->

```http
HTTP/1.1 201 Created

{
    "id": "0x0101",
    "description": "Create a new custom CSR JavaScript Display Template.",
    "group": "Display Template Content Types",
    "hidden": false,
    "name": "JavaScript Display Template",
    "parentId": "0x01",
    "readOnly": false,
    "sealed": false,
    "base": {
        "id": "0x01",
        "description": "Create a new custom CSR JavaScript Display Template.",
        "group": "Display Template Content Types",
        "hidden": false,
        "name": "JavaScript Display Template",
        "readOnly": false,
        "sealed": false
    }
}
```

[site]: ../resources/site.md
[list]: ../resources/list.md
[contentType]: ../resources/contentType.md
