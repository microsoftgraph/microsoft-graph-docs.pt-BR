---
author: swapnil1993
title: Criar contentType
description: Crie um tipo de conteúdo para um site.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 9617d43291e241bb937e7743dcbfddbb83cb6edd
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202045"
---
# <a name="create-contenttype"></a><span data-ttu-id="a31a7-103">Criar contentType</span><span class="sxs-lookup"><span data-stu-id="a31a7-103">Create contentType</span></span>
<span data-ttu-id="a31a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a31a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a31a7-105">Crie um novo [contentType][] para um [site][].</span><span class="sxs-lookup"><span data-stu-id="a31a7-105">Create a new [contentType][] for a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="a31a7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a31a7-106">Permissions</span></span>

<span data-ttu-id="a31a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a31a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a31a7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a31a7-109">Permission type</span></span>      | <span data-ttu-id="a31a7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a31a7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a31a7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a31a7-111">Delegated (work or school account)</span></span> |<span data-ttu-id="a31a7-112">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a31a7-112">Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="a31a7-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a31a7-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="a31a7-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="a31a7-114">Not Supported</span></span>    |
|<span data-ttu-id="a31a7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a31a7-115">Application</span></span> |<span data-ttu-id="a31a7-116">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a31a7-116">Sites.Manage.All, Sites.FullControl.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="a31a7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a31a7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/contentTypes

```

## <a name="request-headers"></a><span data-ttu-id="a31a7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a31a7-118">Request headers</span></span>
|<span data-ttu-id="a31a7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a31a7-119">Name</span></span>|<span data-ttu-id="a31a7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a31a7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a31a7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a31a7-121">Authorization</span></span>|<span data-ttu-id="a31a7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a31a7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a31a7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a31a7-124">Content-Type</span></span>|<span data-ttu-id="a31a7-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a31a7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a31a7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a31a7-127">Request body</span></span>

<span data-ttu-id="a31a7-128">No corpo da solicitação, fornece uma representação JSON do [recurso contentType][] a ser criado.</span><span class="sxs-lookup"><span data-stu-id="a31a7-128">In the request body, supply a JSON representation of the [contentType][] resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="a31a7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a31a7-129">Response</span></span>

<span data-ttu-id="a31a7-130">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [contentType][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a31a7-130">If successful, this method returns a `201 Created` response code and a [contentType][] object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="a31a7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a31a7-131">Example</span></span>

<span data-ttu-id="a31a7-132">O exemplo a seguir mostra como criar um novo tipo de conteúdo genérico.</span><span class="sxs-lookup"><span data-stu-id="a31a7-132">The following example shows how to create a new generic content type.</span></span>

### <a name="request"></a><span data-ttu-id="a31a7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a31a7-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a31a7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a31a7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contenttype"
}
-->

```http
POST https://graph.microsoft.com/beta/sites/{id}/contentTypes
Content-Type: application/json

{
    "name": "docSet",
    "description": "custom docset",
    "base": {
        "name": "Document Set",
        "id": "0x0120D520"
    },
    "group": "Document Set Content Types" 
}
```
# <a name="javascript"></a>[<span data-ttu-id="a31a7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a31a7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="a31a7-136">C#</span><span class="sxs-lookup"><span data-stu-id="a31a7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a31a7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a31a7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a31a7-138">Java</span><span class="sxs-lookup"><span data-stu-id="a31a7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a31a7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a31a7-139">Response</span></span>
><span data-ttu-id="a31a7-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a31a7-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "0x01002A2479FF33DD4BC3B1533A012B653717",
  "name": "docSet",
  "group":"Document Set Content Types",
  "description" : "custom docset",
  "base": {
        "name": "Document Set",
        "id": "0x0120D520"
   }
}
```


[contentType]: ../resources/contentType.md
[site]: ../resources/site.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a Content type in a site",
  "keywords": "content type",
  "section": "documentation",
  "tocPath": "sites/Create ContentType",
  "suppressions": [
  ]
}
-->
