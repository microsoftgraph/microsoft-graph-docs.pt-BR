---
author: JeremyKelley
title: Remover item do pacote
description: Remover item de um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: edd7647be648b5eda1560157d35c6a7b2d4aa130
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50774359"
---
# <a name="remove-item-from-bundle"></a><span data-ttu-id="6d482-103">Remover item do pacote</span><span class="sxs-lookup"><span data-stu-id="6d482-103">Remove item from bundle</span></span>

<span data-ttu-id="6d482-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d482-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d482-105">Remover um item de um [pacote][].</span><span class="sxs-lookup"><span data-stu-id="6d482-105">Remove an item from a [bundle][].</span></span>

## <a name="permissions"></a><span data-ttu-id="6d482-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d482-106">Permissions</span></span>

<span data-ttu-id="6d482-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d482-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d482-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d482-109">Permission type</span></span>      | <span data-ttu-id="6d482-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d482-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d482-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d482-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6d482-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d482-112">Not supported.</span></span>                             |
|<span data-ttu-id="6d482-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d482-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d482-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d482-114">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="6d482-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d482-115">Application</span></span>          | <span data-ttu-id="6d482-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d482-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="6d482-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d482-117">HTTP request</span></span>

```http
DELETE /drive/bundles/{bundle-id}/children/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="6d482-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d482-118">Request headers</span></span>

| <span data-ttu-id="6d482-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6d482-119">Name</span></span>          | <span data-ttu-id="6d482-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d482-120">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="6d482-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d482-121">Authorization</span></span> | <span data-ttu-id="6d482-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="6d482-122">Bearer \{token\}.</span></span> <span data-ttu-id="6d482-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d482-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d482-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d482-124">Request body</span></span>

<span data-ttu-id="6d482-125">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="6d482-125">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d482-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d482-126">Response</span></span>

<span data-ttu-id="6d482-127">Se tiver êxito, a resposta será `204 No Content` .</span><span class="sxs-lookup"><span data-stu-id="6d482-127">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="6d482-128">Leia o tópico [Respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="6d482-128">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="6d482-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d482-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d482-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d482-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6d482-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d482-131">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "remove-from-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children/{item-id}
```
# <a name="c"></a>[<span data-ttu-id="6d482-132">C#</span><span class="sxs-lookup"><span data-stu-id="6d482-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-from-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d482-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d482-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-from-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d482-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d482-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-from-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6d482-135">Java</span><span class="sxs-lookup"><span data-stu-id="6d482-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-from-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6d482-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d482-136">Response</span></span>

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


