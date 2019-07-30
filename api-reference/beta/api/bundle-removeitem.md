---
author: JeremyKelley
ms.author: jeremyke
title: Remover item do pacote
description: Remover item de um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 26c965725044d09eb4b22807ad37aa15353e0513
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932594"
---
# <a name="remove-item-from-bundle"></a><span data-ttu-id="cc00b-103">Remover item do pacote</span><span class="sxs-lookup"><span data-stu-id="cc00b-103">Remove item from bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc00b-104">Remover um item de um [pacote][].</span><span class="sxs-lookup"><span data-stu-id="cc00b-104">Remove an item from a [bundle][].</span></span>

## <a name="permissions"></a><span data-ttu-id="cc00b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc00b-105">Permissions</span></span>

<span data-ttu-id="cc00b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc00b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc00b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc00b-108">Permission type</span></span>      | <span data-ttu-id="cc00b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc00b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc00b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc00b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cc00b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc00b-111">Not supported.</span></span>                             |
|<span data-ttu-id="cc00b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc00b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc00b-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc00b-113">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="cc00b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc00b-114">Application</span></span>          | <span data-ttu-id="cc00b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc00b-115">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="cc00b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc00b-116">HTTP request</span></span>

```http
DELETE /drive/bundles/{bundle-id}/children/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="cc00b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc00b-117">Request headers</span></span>

| <span data-ttu-id="cc00b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="cc00b-118">Name</span></span>          | <span data-ttu-id="cc00b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc00b-119">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="cc00b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc00b-120">Authorization</span></span> | <span data-ttu-id="cc00b-121">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="cc00b-121">Bearer \{token\}.</span></span> <span data-ttu-id="cc00b-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc00b-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc00b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc00b-123">Request body</span></span>

<span data-ttu-id="cc00b-124">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="cc00b-124">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc00b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc00b-125">Response</span></span>

<span data-ttu-id="cc00b-126">Se tiver êxito, a resposta `204 No Content`será.</span><span class="sxs-lookup"><span data-stu-id="cc00b-126">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="cc00b-127">Leia o tópico [respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="cc00b-127">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="cc00b-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc00b-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc00b-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc00b-129">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cc00b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc00b-130">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "remove-from-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cc00b-131">C#</span><span class="sxs-lookup"><span data-stu-id="cc00b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-from-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cc00b-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="cc00b-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-from-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cc00b-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="cc00b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-from-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cc00b-134">Java</span><span class="sxs-lookup"><span data-stu-id="cc00b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-from-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cc00b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc00b-135">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


[pacote]: ../resources/bundle.md
[bundle]: ../resources/bundle.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Remove an item from a bundle.",
  "keywords": "",
  "section": "documentation"
} -->
