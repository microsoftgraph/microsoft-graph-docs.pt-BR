---
title: Excluir namedLocation
description: Excluir um objeto namedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9c5fb698736bf6c365f7956a3738e24f85ed479e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937963"
---
# <a name="delete-namedlocation"></a><span data-ttu-id="d9709-103">Excluir namedLocation</span><span class="sxs-lookup"><span data-stu-id="d9709-103">Delete namedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9709-104">Excluir um objeto [namedLocation](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="d9709-104">Delete a [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9709-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9709-105">Permissions</span></span>

<span data-ttu-id="d9709-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9709-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d9709-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9709-108">Permission type</span></span>                        | <span data-ttu-id="d9709-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9709-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d9709-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9709-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9709-111">Policy. ReadWrite. ConditionalAccess e Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="d9709-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="d9709-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9709-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9709-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9709-113">Not supported.</span></span> |
| <span data-ttu-id="d9709-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9709-114">Application</span></span>                            | <span data-ttu-id="d9709-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9709-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="d9709-116">Essa API requer várias permissões.</span><span class="sxs-lookup"><span data-stu-id="d9709-116">This API requires multiple permissions.</span></span> <span data-ttu-id="d9709-117">Para obter detalhes, consulte [known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="d9709-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="d9709-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9709-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d9709-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9709-119">Request headers</span></span>

| <span data-ttu-id="d9709-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d9709-120">Name</span></span>          | <span data-ttu-id="d9709-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9709-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d9709-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9709-122">Authorization</span></span> | <span data-ttu-id="d9709-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9709-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9709-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9709-125">Request body</span></span>

<span data-ttu-id="d9709-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9709-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9709-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9709-127">Response</span></span>

<span data-ttu-id="d9709-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9709-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9709-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d9709-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9709-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9709-131">Request</span></span>

<span data-ttu-id="d9709-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9709-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d9709-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9709-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_namedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d9709-134">C#</span><span class="sxs-lookup"><span data-stu-id="d9709-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-namedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d9709-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9709-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-namedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d9709-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9709-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-namedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d9709-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9709-137">Response</span></span>

<span data-ttu-id="d9709-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9709-138">The following is an example of the response.</span></span>

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
  "description": "Delete namedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
