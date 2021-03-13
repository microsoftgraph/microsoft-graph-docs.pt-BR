---
author: swapnil1993
title: Obter columnDefinition
description: " Obter uma coluna de tipo de conteúdo."
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 9eaa0065d6f5f677ac603df115748a75038adea9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770872"
---
# <a name="get-columndefinition"></a><span data-ttu-id="0e658-103">Obter columnDefinition</span><span class="sxs-lookup"><span data-stu-id="0e658-103">Get columnDefinition</span></span>
<span data-ttu-id="0e658-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e658-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="0e658-105">Recupere os metadados de uma [coluna contentType][] [.][columnDefinition]</span><span class="sxs-lookup"><span data-stu-id="0e658-105">Retrieve the metadata for a [contentType][] [column][columnDefinition].</span></span>

  

## <a name="permissions"></a><span data-ttu-id="0e658-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e658-106">Permissions</span></span>

  

<span data-ttu-id="0e658-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0e658-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="0e658-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e658-109">Permission type</span></span> | <span data-ttu-id="0e658-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e658-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e658-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e658-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0e658-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0e658-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="0e658-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e658-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e658-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e658-114">Not supported.</span></span> |
|<span data-ttu-id="0e658-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e658-115">Application</span></span> | <span data-ttu-id="0e658-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0e658-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |

  

## <a name="http-request"></a><span data-ttu-id="0e658-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e658-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http

GET /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
GET /sites/{site-id}/lists/{list-id}//contentTypes/{contentType-id}/columns/{column-id}
```

## <a name="request-headers"></a><span data-ttu-id="0e658-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e658-118">Request headers</span></span>
|<span data-ttu-id="0e658-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0e658-119">Name</span></span>|<span data-ttu-id="0e658-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e658-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0e658-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e658-121">Authorization</span></span>|<span data-ttu-id="0e658-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e658-p102">Bearer {token}. Required.</span></span>|  

## <a name="request-body"></a><span data-ttu-id="0e658-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e658-124">Request body</span></span>

  

<span data-ttu-id="0e658-125">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="0e658-125">Do not supply a request body with this method.</span></span>

  

## <a name="example"></a><span data-ttu-id="0e658-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e658-126">Example</span></span>

  

### <a name="request"></a><span data-ttu-id="0e658-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e658-127">Request</span></span>

  


# <a name="http"></a>[<span data-ttu-id="0e658-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e658-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_column_from_contenttype" } -->

  

```msgraph-interactive
GET /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
```
# <a name="c"></a>[<span data-ttu-id="0e658-129">C#</span><span class="sxs-lookup"><span data-stu-id="0e658-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-column-from-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e658-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e658-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-column-from-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e658-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e658-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-column-from-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e658-132">Java</span><span class="sxs-lookup"><span data-stu-id="0e658-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-column-from-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


  

#### <a name="response"></a><span data-ttu-id="0e658-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e658-133">Response</span></span>

  

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true } -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Title",
  "hidden": false,
  "id": "99ddcf45-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Title",
  "readOnly": false,
  "required": false,
  "text": {
    "allowMultipleLines": false,
    "appendChangesToExistingText": false,
    "linesForEditing": 0,
    "maxLength": 255
  }
}
```

  

[columnDefinition]: ../resources/columnDefinition.md

[list]: ../resources/list.md

[site]: ../resources/site.md

[contentType]: ../resources/contentType.md
  
