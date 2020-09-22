---
author: JeremyKelley
ms.author: jeremyke
title: Adicionar item a um pacote
description: Adicionar item a um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 910054e5077c8d69939a14c42db824dd862141d8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987773"
---
# <a name="add-item-to-a-bundle"></a><span data-ttu-id="021c4-103">Adicionar item a um pacote</span><span class="sxs-lookup"><span data-stu-id="021c4-103">Add item to a bundle</span></span>

<span data-ttu-id="021c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="021c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="021c4-105">Adicione um [driveItem][] adicional de uma unidade a um [pacote][].</span><span class="sxs-lookup"><span data-stu-id="021c4-105">Add an additional [driveItem][] from a drive to a [bundle][].</span></span>

[pacote]: ../resources/bundle.md
[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a><span data-ttu-id="021c4-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="021c4-108">Permissions</span></span>

<span data-ttu-id="021c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="021c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="021c4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="021c4-111">Permission type</span></span>      | <span data-ttu-id="021c4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="021c4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="021c4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="021c4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="021c4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="021c4-114">Not supported.</span></span>                             |
|<span data-ttu-id="021c4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="021c4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="021c4-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="021c4-116">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="021c4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="021c4-117">Application</span></span>          | <span data-ttu-id="021c4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="021c4-118">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="021c4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="021c4-119">HTTP request</span></span>

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a><span data-ttu-id="021c4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="021c4-120">Request headers</span></span>

| <span data-ttu-id="021c4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="021c4-121">Name</span></span>          | <span data-ttu-id="021c4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="021c4-122">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="021c4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="021c4-123">Authorization</span></span> | <span data-ttu-id="021c4-124">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="021c4-124">Bearer \{token\}.</span></span> <span data-ttu-id="021c4-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="021c4-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="021c4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="021c4-126">Request body</span></span>

<span data-ttu-id="021c4-127">O corpo da solicitação inclui o identificador de um item que deve ser adicionado à coleção Children do pacote.</span><span class="sxs-lookup"><span data-stu-id="021c4-127">The request body includes the identifier for an item that should be added to the bundle's children collection.</span></span>

## <a name="response"></a><span data-ttu-id="021c4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="021c4-128">Response</span></span>

<span data-ttu-id="021c4-129">Se tiver êxito, a resposta será `204 No Content` .</span><span class="sxs-lookup"><span data-stu-id="021c4-129">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="021c4-130">Veja mais informações sobre como os erros são retornados no tópico [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="021c4-130">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="021c4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="021c4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="021c4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="021c4-132">Request</span></span>

<span data-ttu-id="021c4-133">Essa solicitação adicionará um item existente ao pacote especificado.</span><span class="sxs-lookup"><span data-stu-id="021c4-133">This request will add an existing item to the specified bundle.</span></span>


# <a name="http"></a>[<span data-ttu-id="021c4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="021c4-134">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```
# <a name="c"></a>[<span data-ttu-id="021c4-135">C#</span><span class="sxs-lookup"><span data-stu-id="021c4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-to-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="021c4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="021c4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-to-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="021c4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="021c4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-to-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="021c4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="021c4-138">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Add items to an existing bundle.",
  "keywords": "",
  "section": "documentation"
} -->


