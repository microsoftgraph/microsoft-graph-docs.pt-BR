---
title: Excluir o external
description: Exclui um objeto de um.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7cf287b7886cc9f0ee5cdb0d3e20ee5e43cb4ce5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954638"
---
# <a name="delete-externalgroup"></a><span data-ttu-id="4f388-103">Excluir o external</span><span class="sxs-lookup"><span data-stu-id="4f388-103">Delete externalGroup</span></span>

<span data-ttu-id="4f388-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f388-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f388-105">Excluir um [objeto](../resources/externalgroup.md) de um.</span><span class="sxs-lookup"><span data-stu-id="4f388-105">Delete an [externalGroup](../resources/externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f388-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f388-106">Permissions</span></span>

<span data-ttu-id="4f388-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f388-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f388-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f388-109">Permission type</span></span>                        | <span data-ttu-id="4f388-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f388-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4f388-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f388-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f388-112">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4f388-112">Not supported</span></span>                               |
| <span data-ttu-id="4f388-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f388-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f388-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4f388-114">Not supported</span></span>                               |
| <span data-ttu-id="4f388-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f388-115">Application</span></span>                            | <span data-ttu-id="4f388-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f388-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="4f388-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f388-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="4f388-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f388-118">Request headers</span></span>

| <span data-ttu-id="4f388-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4f388-119">Name</span></span>          | <span data-ttu-id="4f388-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f388-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4f388-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f388-121">Authorization</span></span> | <span data-ttu-id="4f388-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f388-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f388-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f388-124">Request body</span></span>

<span data-ttu-id="4f388-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f388-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f388-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f388-126">Response</span></span>

<span data-ttu-id="4f388-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4f388-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4f388-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4f388-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4f388-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f388-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4f388-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f388-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalgroup"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000
```
# <a name="c"></a>[<span data-ttu-id="4f388-131">C#</span><span class="sxs-lookup"><span data-stu-id="4f388-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f388-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f388-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f388-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f388-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f388-134">Java</span><span class="sxs-lookup"><span data-stu-id="4f388-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="4f388-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f388-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
