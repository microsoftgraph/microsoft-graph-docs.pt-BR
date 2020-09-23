---
title: Excluir o external
description: Exclui um objeto de um.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 43fb3f0cb0740fe3c7fef23bb244681967cbb13d
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223048"
---
# <a name="delete-externalgroup"></a><span data-ttu-id="108ad-103">Excluir o external</span><span class="sxs-lookup"><span data-stu-id="108ad-103">Delete externalGroup</span></span>

<span data-ttu-id="108ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="108ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="108ad-105">Excluir um [objeto](../resources/externalgroup.md) de um.</span><span class="sxs-lookup"><span data-stu-id="108ad-105">Delete an [externalGroup](../resources/externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="108ad-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="108ad-106">Permissions</span></span>

<span data-ttu-id="108ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="108ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="108ad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="108ad-109">Permission type</span></span>                        | <span data-ttu-id="108ad-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="108ad-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="108ad-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="108ad-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="108ad-112">Incompatível</span><span class="sxs-lookup"><span data-stu-id="108ad-112">Not supported</span></span>                               |
| <span data-ttu-id="108ad-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="108ad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="108ad-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="108ad-114">Not supported</span></span>                               |
| <span data-ttu-id="108ad-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="108ad-115">Application</span></span>                            | <span data-ttu-id="108ad-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="108ad-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="108ad-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="108ad-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="108ad-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="108ad-118">Request headers</span></span>

| <span data-ttu-id="108ad-119">Nome</span><span class="sxs-lookup"><span data-stu-id="108ad-119">Name</span></span>          | <span data-ttu-id="108ad-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="108ad-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="108ad-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="108ad-121">Authorization</span></span> | <span data-ttu-id="108ad-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="108ad-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="108ad-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="108ad-124">Request body</span></span>

<span data-ttu-id="108ad-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="108ad-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="108ad-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="108ad-126">Response</span></span>

<span data-ttu-id="108ad-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="108ad-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="108ad-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="108ad-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="108ad-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="108ad-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="108ad-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="108ad-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalgroup"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000
```
# <a name="c"></a>[<span data-ttu-id="108ad-131">C#</span><span class="sxs-lookup"><span data-stu-id="108ad-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="108ad-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="108ad-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="108ad-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="108ad-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="108ad-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="108ad-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
