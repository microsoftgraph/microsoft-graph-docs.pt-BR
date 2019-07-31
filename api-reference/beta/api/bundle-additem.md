---
author: JeremyKelley
ms.author: jeremyke
title: Adicionar item a um pacote
description: Adicionar item a um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: f6680d4903111301f61f11f1975596386dd263be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944839"
---
# <a name="add-item-to-a-bundle"></a><span data-ttu-id="7bc6f-103">Adicionar item a um pacote</span><span class="sxs-lookup"><span data-stu-id="7bc6f-103">Add item to a bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bc6f-104">Adicione um [driveItem][] adicional de uma unidade a um [pacote][].</span><span class="sxs-lookup"><span data-stu-id="7bc6f-104">Add an additional [driveItem][] from a drive to a [bundle][].</span></span>

[pacote]: ../resources/bundle.md
[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a><span data-ttu-id="7bc6f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7bc6f-107">Permissions</span></span>

<span data-ttu-id="7bc6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bc6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bc6f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bc6f-110">Permission type</span></span>      | <span data-ttu-id="7bc6f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7bc6f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bc6f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bc6f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7bc6f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bc6f-113">Not supported.</span></span>                             |
|<span data-ttu-id="7bc6f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bc6f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bc6f-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bc6f-115">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="7bc6f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bc6f-116">Application</span></span>          | <span data-ttu-id="7bc6f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bc6f-117">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="7bc6f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bc6f-118">HTTP request</span></span>

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a><span data-ttu-id="7bc6f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bc6f-119">Request headers</span></span>

| <span data-ttu-id="7bc6f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7bc6f-120">Name</span></span>          | <span data-ttu-id="7bc6f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bc6f-121">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="7bc6f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bc6f-122">Authorization</span></span> | <span data-ttu-id="7bc6f-123">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="7bc6f-123">Bearer \{token\}.</span></span> <span data-ttu-id="7bc6f-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bc6f-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bc6f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bc6f-125">Request body</span></span>

<span data-ttu-id="7bc6f-126">O corpo da solicitação inclui o identificador de um item que deve ser adicionado à coleção Children do pacote.</span><span class="sxs-lookup"><span data-stu-id="7bc6f-126">The request body includes the identifier for an item that should be added to the bundle's children collection.</span></span>

## <a name="response"></a><span data-ttu-id="7bc6f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bc6f-127">Response</span></span>

<span data-ttu-id="7bc6f-128">Se tiver êxito, a resposta `204 No Content`será.</span><span class="sxs-lookup"><span data-stu-id="7bc6f-128">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="7bc6f-129">Veja mais informações sobre como os erros são retornados no tópico [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="7bc6f-129">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="7bc6f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7bc6f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bc6f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bc6f-131">Request</span></span>

<span data-ttu-id="7bc6f-132">Essa solicitação adicionará um item existente ao pacote especificado.</span><span class="sxs-lookup"><span data-stu-id="7bc6f-132">This request will add an existing item to the specified bundle.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7bc6f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bc6f-133">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7bc6f-134">C#</span><span class="sxs-lookup"><span data-stu-id="7bc6f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-to-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bc6f-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="7bc6f-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-to-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7bc6f-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7bc6f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-to-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7bc6f-137">Java</span><span class="sxs-lookup"><span data-stu-id="7bc6f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-to-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7bc6f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bc6f-138">Response</span></span>

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
