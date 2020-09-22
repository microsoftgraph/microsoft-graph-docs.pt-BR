---
title: Excluir termo
description: Excluir um objeto Term.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: bd694ac1d97b24652387e75f14c4f29d38dd3eb0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044257"
---
# <a name="delete-term"></a><span data-ttu-id="6129b-103">Excluir termo</span><span class="sxs-lookup"><span data-stu-id="6129b-103">Delete term</span></span>
<span data-ttu-id="6129b-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="6129b-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6129b-105">Excluir um objeto [Term](../resources/termstore-term.md) .</span><span class="sxs-lookup"><span data-stu-id="6129b-105">Delete a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6129b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6129b-106">Permissions</span></span>
<span data-ttu-id="6129b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6129b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6129b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6129b-109">Permission type</span></span>|<span data-ttu-id="6129b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6129b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6129b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6129b-111">Delegated (work or school account)</span></span> |<span data-ttu-id="6129b-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6129b-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="6129b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6129b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6129b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6129b-114">Not supported.</span></span>    |
|<span data-ttu-id="6129b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6129b-115">Application</span></span> | <span data-ttu-id="6129b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6129b-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="6129b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6129b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/sets/{setId}/terms/{termId}
```

## <a name="request-headers"></a><span data-ttu-id="6129b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6129b-118">Request headers</span></span>
|<span data-ttu-id="6129b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6129b-119">Name</span></span>|<span data-ttu-id="6129b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6129b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6129b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6129b-121">Authorization</span></span>|<span data-ttu-id="6129b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6129b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6129b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6129b-124">Request body</span></span>
<span data-ttu-id="6129b-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6129b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6129b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6129b-126">Response</span></span>

<span data-ttu-id="6129b-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6129b-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6129b-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6129b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6129b-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6129b-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6129b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="6129b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_term"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/sets/{setId}/terms/{termId}
```
# <a name="c"></a>[<span data-ttu-id="6129b-131">C#</span><span class="sxs-lookup"><span data-stu-id="6129b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-term-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6129b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6129b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-term-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6129b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6129b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-term-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6129b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6129b-134">Response</span></span>
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


