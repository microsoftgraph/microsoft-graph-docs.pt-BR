---
title: Excluir claimsMappingPolicy
description: Exclua claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5749effbb234444cf3ba609df58a0af598c9b204
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863821"
---
# <a name="delete-claimsmappingpolicy"></a><span data-ttu-id="4a517-103">Excluir claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="4a517-103">Delete claimsMappingPolicy</span></span>

<span data-ttu-id="4a517-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a517-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4a517-105">Excluir um objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="4a517-105">Delete a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a517-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a517-106">Permissions</span></span>

<span data-ttu-id="4a517-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="4a517-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4a517-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a517-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a517-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a517-109">Permission type</span></span>                        | <span data-ttu-id="4a517-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a517-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4a517-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a517-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a517-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="4a517-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="4a517-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a517-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a517-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a517-114">Not supported.</span></span> |
| <span data-ttu-id="4a517-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a517-115">Application</span></span>                            | <span data-ttu-id="4a517-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="4a517-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a517-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a517-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4a517-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a517-118">Request headers</span></span>

| <span data-ttu-id="4a517-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4a517-119">Name</span></span>          | <span data-ttu-id="4a517-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a517-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4a517-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a517-121">Authorization</span></span> | <span data-ttu-id="4a517-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="4a517-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a517-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a517-123">Request body</span></span>

<span data-ttu-id="4a517-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4a517-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a517-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a517-125">Response</span></span>

<span data-ttu-id="4a517-126">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4a517-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4a517-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4a517-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4a517-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a517-128">Request</span></span>

<span data-ttu-id="4a517-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a517-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a517-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a517-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="4a517-131">C#</span><span class="sxs-lookup"><span data-stu-id="4a517-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a517-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a517-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a517-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a517-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a517-134">Java</span><span class="sxs-lookup"><span data-stu-id="4a517-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-claimsmappingpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4a517-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a517-135">Response</span></span>

<span data-ttu-id="4a517-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a517-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
