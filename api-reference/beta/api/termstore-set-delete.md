---
title: Excluir conjunto
description: Exclua um objeto set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5dedcb12502dc9877bd63519022dc69149a18bb5
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874421"
---
# <a name="delete-set"></a><span data-ttu-id="c4f92-103">Excluir conjunto</span><span class="sxs-lookup"><span data-stu-id="c4f92-103">Delete set</span></span>
<span data-ttu-id="c4f92-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="c4f92-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4f92-105">Exclua [um objeto](../resources/termstore-set.md) set.</span><span class="sxs-lookup"><span data-stu-id="c4f92-105">Delete a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4f92-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4f92-106">Permissions</span></span>
<span data-ttu-id="c4f92-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4f92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4f92-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4f92-109">Permission type</span></span>|<span data-ttu-id="c4f92-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4f92-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4f92-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4f92-111">Delegated (work or school account)</span></span> |<span data-ttu-id="c4f92-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4f92-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="c4f92-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4f92-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4f92-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4f92-114">Not supported.</span></span>    |
|<span data-ttu-id="c4f92-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4f92-115">Application</span></span> | <span data-ttu-id="c4f92-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4f92-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="c4f92-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4f92-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/sets/{setId}
```

## <a name="request-headers"></a><span data-ttu-id="c4f92-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4f92-118">Request headers</span></span>
|<span data-ttu-id="c4f92-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c4f92-119">Name</span></span>|<span data-ttu-id="c4f92-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4f92-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c4f92-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4f92-121">Authorization</span></span>|<span data-ttu-id="c4f92-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4f92-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4f92-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4f92-124">Request body</span></span>
<span data-ttu-id="c4f92-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4f92-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4f92-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4f92-126">Response</span></span>

<span data-ttu-id="c4f92-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c4f92-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c4f92-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c4f92-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4f92-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4f92-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c4f92-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4f92-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_set"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/sets/{setId}
```
# <a name="c"></a>[<span data-ttu-id="c4f92-131">C#</span><span class="sxs-lookup"><span data-stu-id="c4f92-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4f92-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4f92-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4f92-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4f92-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4f92-134">Java</span><span class="sxs-lookup"><span data-stu-id="c4f92-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-set-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c4f92-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4f92-135">Response</span></span>

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


