---
author: JeremyKelley
ms.author: jeremyke
title: Adicionar item a um pacote
description: Adicionar item a um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c192014a00e3a2119691857c8350dc03d53e1980
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441050"
---
# <a name="add-item-to-a-bundle"></a><span data-ttu-id="8d01e-103">Adicionar item a um pacote</span><span class="sxs-lookup"><span data-stu-id="8d01e-103">Add item to a bundle</span></span>

<span data-ttu-id="8d01e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8d01e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d01e-105">Adicione um [driveItem][] adicional de uma unidade a um [pacote][].</span><span class="sxs-lookup"><span data-stu-id="8d01e-105">Add an additional [driveItem][] from a drive to a [bundle][].</span></span>

[pacote]: ../resources/bundle.md
[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a><span data-ttu-id="8d01e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d01e-108">Permissions</span></span>

<span data-ttu-id="8d01e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d01e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d01e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d01e-111">Permission type</span></span>      | <span data-ttu-id="8d01e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d01e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d01e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d01e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8d01e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d01e-114">Not supported.</span></span>                             |
|<span data-ttu-id="8d01e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d01e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d01e-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d01e-116">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="8d01e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d01e-117">Application</span></span>          | <span data-ttu-id="8d01e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d01e-118">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="8d01e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d01e-119">HTTP request</span></span>

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a><span data-ttu-id="8d01e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d01e-120">Request headers</span></span>

| <span data-ttu-id="8d01e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8d01e-121">Name</span></span>          | <span data-ttu-id="8d01e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d01e-122">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="8d01e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d01e-123">Authorization</span></span> | <span data-ttu-id="8d01e-124">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="8d01e-124">Bearer \{token\}.</span></span> <span data-ttu-id="8d01e-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d01e-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d01e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d01e-126">Request body</span></span>

<span data-ttu-id="8d01e-127">O corpo da solicitação inclui o identificador de um item que deve ser adicionado à coleção Children do pacote.</span><span class="sxs-lookup"><span data-stu-id="8d01e-127">The request body includes the identifier for an item that should be added to the bundle's children collection.</span></span>

## <a name="response"></a><span data-ttu-id="8d01e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d01e-128">Response</span></span>

<span data-ttu-id="8d01e-129">Se tiver êxito, a resposta `204 No Content`será.</span><span class="sxs-lookup"><span data-stu-id="8d01e-129">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="8d01e-130">Veja mais informações sobre como os erros são retornados no tópico [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="8d01e-130">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="8d01e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d01e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d01e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d01e-132">Request</span></span>

<span data-ttu-id="8d01e-133">Essa solicitação adicionará um item existente ao pacote especificado.</span><span class="sxs-lookup"><span data-stu-id="8d01e-133">This request will add an existing item to the specified bundle.</span></span>


# <a name="http"></a>[<span data-ttu-id="8d01e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d01e-134">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```
# <a name="c"></a>[<span data-ttu-id="8d01e-135">C#</span><span class="sxs-lookup"><span data-stu-id="8d01e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-to-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d01e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d01e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-to-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d01e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d01e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-to-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8d01e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d01e-138">Response</span></span>

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
