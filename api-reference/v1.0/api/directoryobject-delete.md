---
title: Excluir directoryObject
description: Exclui um directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a5855a454156509818951cf3e6b8d570b1b9d8bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026089"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="a82dc-103">Excluir directoryObject</span><span class="sxs-lookup"><span data-stu-id="a82dc-103">Delete directoryObject</span></span>

<span data-ttu-id="a82dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a82dc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a82dc-105">Exclui um directoryObject.</span><span class="sxs-lookup"><span data-stu-id="a82dc-105">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="a82dc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a82dc-106">Permissions</span></span>
<span data-ttu-id="a82dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a82dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a82dc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a82dc-109">Permission type</span></span>      | <span data-ttu-id="a82dc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a82dc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a82dc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a82dc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a82dc-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a82dc-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a82dc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a82dc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a82dc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a82dc-114">Not supported.</span></span>    |
|<span data-ttu-id="a82dc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a82dc-115">Application</span></span> | <span data-ttu-id="a82dc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a82dc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a82dc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a82dc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="a82dc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a82dc-118">Request headers</span></span>
| <span data-ttu-id="a82dc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a82dc-119">Name</span></span>       | <span data-ttu-id="a82dc-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a82dc-120">Type</span></span> | <span data-ttu-id="a82dc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a82dc-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a82dc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a82dc-122">Authorization</span></span>  | <span data-ttu-id="a82dc-123">string</span><span class="sxs-lookup"><span data-stu-id="a82dc-123">string</span></span>  | <span data-ttu-id="a82dc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a82dc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a82dc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a82dc-126">Request body</span></span>
<span data-ttu-id="a82dc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a82dc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a82dc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a82dc-128">Response</span></span>

<span data-ttu-id="a82dc-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a82dc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a82dc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a82dc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a82dc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a82dc-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a82dc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a82dc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
# <a name="c"></a>[<span data-ttu-id="a82dc-134">C#</span><span class="sxs-lookup"><span data-stu-id="a82dc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a82dc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a82dc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a82dc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a82dc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a82dc-137">Java</span><span class="sxs-lookup"><span data-stu-id="a82dc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a82dc-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a82dc-138">Response</span></span>

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

