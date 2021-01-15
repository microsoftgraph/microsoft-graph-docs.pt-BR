---
title: Excluir externalGroupMember
description: Exclua um objeto externalGroupMember.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 24bfa2da5277192f4f14e828a7e6ea2d5b5d9ce1
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873168"
---
# <a name="delete-externalgroupmember"></a><span data-ttu-id="b6a0a-103">Excluir externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="b6a0a-103">Delete externalGroupMember</span></span>

<span data-ttu-id="b6a0a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6a0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6a0a-105">[Exclua um objeto externalGroupMember.](../resources/externalgroupmember.md)</span><span class="sxs-lookup"><span data-stu-id="b6a0a-105">Delete an [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6a0a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6a0a-106">Permissions</span></span>

<span data-ttu-id="b6a0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6a0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6a0a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6a0a-109">Permission type</span></span>                        | <span data-ttu-id="b6a0a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6a0a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b6a0a-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6a0a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6a0a-112">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b6a0a-112">Not supported</span></span>                               |
| <span data-ttu-id="b6a0a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6a0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6a0a-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b6a0a-114">Not supported</span></span>                               |
| <span data-ttu-id="b6a0a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6a0a-115">Application</span></span>                            | <span data-ttu-id="b6a0a-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6a0a-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="b6a0a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6a0a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}/members/{externalGroupMemberId}
```

## <a name="request-headers"></a><span data-ttu-id="b6a0a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6a0a-118">Request headers</span></span>

| <span data-ttu-id="b6a0a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b6a0a-119">Name</span></span>          | <span data-ttu-id="b6a0a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6a0a-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b6a0a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6a0a-121">Authorization</span></span> | <span data-ttu-id="b6a0a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6a0a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6a0a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6a0a-124">Request body</span></span>

<span data-ttu-id="b6a0a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6a0a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6a0a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6a0a-126">Response</span></span>

<span data-ttu-id="b6a0a-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b6a0a-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b6a0a-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b6a0a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b6a0a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6a0a-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b6a0a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6a0a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalgroupmember"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members/14m1b9c38qe647f6a
```
# <a name="c"></a>[<span data-ttu-id="b6a0a-131">C#</span><span class="sxs-lookup"><span data-stu-id="b6a0a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalgroupmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6a0a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6a0a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalgroupmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6a0a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6a0a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalgroupmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6a0a-134">Java</span><span class="sxs-lookup"><span data-stu-id="b6a0a-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalgroupmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="b6a0a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6a0a-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
