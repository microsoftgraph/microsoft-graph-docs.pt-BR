---
title: Excluir externalGroup
description: Exclui um objeto externalGroup.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: a039ab9969766a6fa1716c481c0d74f5b8bf125d
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873182"
---
# <a name="delete-externalgroup"></a><span data-ttu-id="0e5a5-103">Excluir externalGroup</span><span class="sxs-lookup"><span data-stu-id="0e5a5-103">Delete externalGroup</span></span>

<span data-ttu-id="0e5a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e5a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e5a5-105">[Exclua um objeto externalGroup.](../resources/externalgroup.md)</span><span class="sxs-lookup"><span data-stu-id="0e5a5-105">Delete an [externalGroup](../resources/externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e5a5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e5a5-106">Permissions</span></span>

<span data-ttu-id="0e5a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e5a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e5a5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e5a5-109">Permission type</span></span>                        | <span data-ttu-id="0e5a5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e5a5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0e5a5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e5a5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e5a5-112">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0e5a5-112">Not supported</span></span>                               |
| <span data-ttu-id="0e5a5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e5a5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e5a5-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0e5a5-114">Not supported</span></span>                               |
| <span data-ttu-id="0e5a5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e5a5-115">Application</span></span>                            | <span data-ttu-id="0e5a5-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e5a5-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="0e5a5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e5a5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="0e5a5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e5a5-118">Request headers</span></span>

| <span data-ttu-id="0e5a5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0e5a5-119">Name</span></span>          | <span data-ttu-id="0e5a5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e5a5-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0e5a5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e5a5-121">Authorization</span></span> | <span data-ttu-id="0e5a5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e5a5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e5a5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e5a5-124">Request body</span></span>

<span data-ttu-id="0e5a5-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e5a5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e5a5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e5a5-126">Response</span></span>

<span data-ttu-id="0e5a5-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0e5a5-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0e5a5-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0e5a5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e5a5-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e5a5-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0e5a5-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e5a5-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalgroup"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000
```
# <a name="c"></a>[<span data-ttu-id="0e5a5-131">C#</span><span class="sxs-lookup"><span data-stu-id="0e5a5-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e5a5-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e5a5-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e5a5-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e5a5-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e5a5-134">Java</span><span class="sxs-lookup"><span data-stu-id="0e5a5-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="0e5a5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e5a5-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
