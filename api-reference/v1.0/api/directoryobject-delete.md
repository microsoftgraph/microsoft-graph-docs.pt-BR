---
title: Excluir directoryObject
description: Exclui um directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: fab6000f09ae96e1a002c3e698d8c92faa015c51
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434451"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="c6579-103">Excluir directoryObject</span><span class="sxs-lookup"><span data-stu-id="c6579-103">Delete directoryObject</span></span>

<span data-ttu-id="c6579-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6579-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c6579-105">Exclui um directoryObject.</span><span class="sxs-lookup"><span data-stu-id="c6579-105">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6579-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6579-106">Permissions</span></span>
<span data-ttu-id="c6579-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6579-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c6579-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6579-109">Permission type</span></span>      | <span data-ttu-id="c6579-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6579-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6579-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6579-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c6579-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c6579-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c6579-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6579-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6579-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6579-114">Not supported.</span></span>    |
|<span data-ttu-id="c6579-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6579-115">Application</span></span> | <span data-ttu-id="c6579-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6579-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6579-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6579-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c6579-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6579-118">Request headers</span></span>
| <span data-ttu-id="c6579-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c6579-119">Name</span></span>       | <span data-ttu-id="c6579-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6579-120">Type</span></span> | <span data-ttu-id="c6579-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6579-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c6579-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6579-122">Authorization</span></span>  | <span data-ttu-id="c6579-123">string</span><span class="sxs-lookup"><span data-stu-id="c6579-123">string</span></span>  | <span data-ttu-id="c6579-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6579-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6579-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6579-126">Request body</span></span>
<span data-ttu-id="c6579-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c6579-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6579-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6579-128">Response</span></span>

<span data-ttu-id="c6579-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6579-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6579-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6579-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6579-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6579-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c6579-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6579-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
# <a name="c"></a>[<span data-ttu-id="c6579-134">C#</span><span class="sxs-lookup"><span data-stu-id="c6579-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6579-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6579-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6579-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6579-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6579-137">Java</span><span class="sxs-lookup"><span data-stu-id="c6579-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c6579-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6579-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

