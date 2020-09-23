---
title: Excluir externalGroupMember
description: Excluir um objeto externalGroupMember.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: dbb4f89522432f083169cc3c559a66a15c2874b3
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223051"
---
# <a name="delete-externalgroupmember"></a><span data-ttu-id="29a40-103">Excluir externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="29a40-103">Delete externalGroupMember</span></span>

<span data-ttu-id="29a40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29a40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29a40-105">Excluir um objeto [externalGroupMember](../resources/externalgroupmember.md) .</span><span class="sxs-lookup"><span data-stu-id="29a40-105">Delete an [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="29a40-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="29a40-106">Permissions</span></span>

<span data-ttu-id="29a40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29a40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29a40-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29a40-109">Permission type</span></span>                        | <span data-ttu-id="29a40-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="29a40-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="29a40-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29a40-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="29a40-112">Incompatível</span><span class="sxs-lookup"><span data-stu-id="29a40-112">Not supported</span></span>                               |
| <span data-ttu-id="29a40-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29a40-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29a40-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="29a40-114">Not supported</span></span>                               |
| <span data-ttu-id="29a40-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29a40-115">Application</span></span>                            | <span data-ttu-id="29a40-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29a40-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="29a40-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29a40-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}/members/{externalGroupMemberId}
```

## <a name="request-headers"></a><span data-ttu-id="29a40-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29a40-118">Request headers</span></span>

| <span data-ttu-id="29a40-119">Nome</span><span class="sxs-lookup"><span data-stu-id="29a40-119">Name</span></span>          | <span data-ttu-id="29a40-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="29a40-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="29a40-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="29a40-121">Authorization</span></span> | <span data-ttu-id="29a40-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29a40-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29a40-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29a40-124">Request body</span></span>

<span data-ttu-id="29a40-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="29a40-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29a40-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="29a40-126">Response</span></span>

<span data-ttu-id="29a40-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="29a40-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="29a40-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="29a40-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="29a40-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29a40-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="29a40-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="29a40-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalgroupmember"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members/14m1b9c38qe647f6a
```
# <a name="c"></a>[<span data-ttu-id="29a40-131">C#</span><span class="sxs-lookup"><span data-stu-id="29a40-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalgroupmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29a40-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29a40-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalgroupmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29a40-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29a40-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalgroupmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="29a40-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="29a40-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
