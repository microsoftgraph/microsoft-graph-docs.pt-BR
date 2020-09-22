---
title: Excluir conjunto
description: Excluir um objeto Set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: bba7bb62b863bbe63b4158fe2706985a4a9bb0d8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055729"
---
# <a name="delete-set"></a><span data-ttu-id="6335a-103">Excluir conjunto</span><span class="sxs-lookup"><span data-stu-id="6335a-103">Delete set</span></span>
<span data-ttu-id="6335a-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="6335a-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6335a-105">Excluir um objeto [set](../resources/termstore-set.md) .</span><span class="sxs-lookup"><span data-stu-id="6335a-105">Delete a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6335a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6335a-106">Permissions</span></span>
<span data-ttu-id="6335a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6335a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6335a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6335a-109">Permission type</span></span>|<span data-ttu-id="6335a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6335a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6335a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6335a-111">Delegated (work or school account)</span></span> |<span data-ttu-id="6335a-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6335a-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="6335a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6335a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6335a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6335a-114">Not supported.</span></span>    |
|<span data-ttu-id="6335a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6335a-115">Application</span></span> | <span data-ttu-id="6335a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6335a-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="6335a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6335a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/sets/{setId}
```

## <a name="request-headers"></a><span data-ttu-id="6335a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6335a-118">Request headers</span></span>
|<span data-ttu-id="6335a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6335a-119">Name</span></span>|<span data-ttu-id="6335a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6335a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6335a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6335a-121">Authorization</span></span>|<span data-ttu-id="6335a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6335a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6335a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6335a-124">Request body</span></span>
<span data-ttu-id="6335a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6335a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6335a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6335a-126">Response</span></span>

<span data-ttu-id="6335a-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6335a-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6335a-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6335a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6335a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6335a-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6335a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="6335a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_set"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/sets/{setId}
```
# <a name="c"></a>[<span data-ttu-id="6335a-131">C#</span><span class="sxs-lookup"><span data-stu-id="6335a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6335a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6335a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6335a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6335a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6335a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6335a-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "Delete a termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Delete termSet",
  "suppressions": [
  ]
}
-->


