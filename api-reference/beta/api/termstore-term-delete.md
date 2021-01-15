---
title: Excluir termo
description: Exclua um objeto term.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 706ad5b9457014de236485f526db994dd8a29866
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874372"
---
# <a name="delete-term"></a><span data-ttu-id="f911e-103">Excluir termo</span><span class="sxs-lookup"><span data-stu-id="f911e-103">Delete term</span></span>
<span data-ttu-id="f911e-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="f911e-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f911e-105">Exclua um [objeto term.](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="f911e-105">Delete a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f911e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f911e-106">Permissions</span></span>
<span data-ttu-id="f911e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f911e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f911e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f911e-109">Permission type</span></span>|<span data-ttu-id="f911e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f911e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f911e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f911e-111">Delegated (work or school account)</span></span> |<span data-ttu-id="f911e-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f911e-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="f911e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f911e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f911e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f911e-114">Not supported.</span></span>    |
|<span data-ttu-id="f911e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f911e-115">Application</span></span> | <span data-ttu-id="f911e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f911e-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="f911e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f911e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/sets/{setId}/terms/{termId}
```

## <a name="request-headers"></a><span data-ttu-id="f911e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f911e-118">Request headers</span></span>
|<span data-ttu-id="f911e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f911e-119">Name</span></span>|<span data-ttu-id="f911e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f911e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f911e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f911e-121">Authorization</span></span>|<span data-ttu-id="f911e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f911e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f911e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f911e-124">Request body</span></span>
<span data-ttu-id="f911e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f911e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f911e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="f911e-126">Response</span></span>

<span data-ttu-id="f911e-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f911e-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f911e-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f911e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f911e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f911e-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f911e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f911e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_term"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/sets/{setId}/terms/{termId}
```
# <a name="c"></a>[<span data-ttu-id="f911e-131">C#</span><span class="sxs-lookup"><span data-stu-id="f911e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-term-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f911e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f911e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-term-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f911e-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f911e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-term-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f911e-134">Java</span><span class="sxs-lookup"><span data-stu-id="f911e-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-term-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f911e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f911e-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Delete a term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Delete term",
  "suppressions": [
  ]
}
-->


