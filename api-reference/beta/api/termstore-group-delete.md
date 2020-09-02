---
title: Excluir grupo
description: Excluir um objeto Group.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: fc013c512016c9ff683b0fe3f0e4c369141ba612
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330260"
---
# <a name="delete-groups"></a><span data-ttu-id="85fee-103">Excluir grupos</span><span class="sxs-lookup"><span data-stu-id="85fee-103">Delete groups</span></span>
<span data-ttu-id="85fee-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="85fee-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85fee-105">Excluir um objeto de [grupo](../resources/termstore-group.md) no [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="85fee-105">Delete a [group](../resources/termstore-group.md) object in the term [store].</span></span>

## <a name="permissions"></a><span data-ttu-id="85fee-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="85fee-106">Permissions</span></span>
<span data-ttu-id="85fee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85fee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85fee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85fee-109">Permission type</span></span>|<span data-ttu-id="85fee-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="85fee-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85fee-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85fee-111">Delegated (work or school account)</span></span> |<span data-ttu-id="85fee-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85fee-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="85fee-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85fee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85fee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85fee-114">Not supported.</span></span>    |
|<span data-ttu-id="85fee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85fee-115">Application</span></span> | <span data-ttu-id="85fee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85fee-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="85fee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85fee-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/groups/{groupId}
```

## <a name="request-headers"></a><span data-ttu-id="85fee-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85fee-118">Request headers</span></span>
|<span data-ttu-id="85fee-119">Nome</span><span class="sxs-lookup"><span data-stu-id="85fee-119">Name</span></span>|<span data-ttu-id="85fee-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="85fee-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="85fee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="85fee-121">Authorization</span></span>|<span data-ttu-id="85fee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85fee-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="85fee-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85fee-124">Request body</span></span>
<span data-ttu-id="85fee-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85fee-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85fee-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="85fee-126">Response</span></span>

<span data-ttu-id="85fee-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="85fee-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="85fee-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="85fee-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="85fee-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85fee-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="85fee-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="85fee-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_from_store"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/groups/{groupId}
```
# <a name="c"></a>[<span data-ttu-id="85fee-131">C#</span><span class="sxs-lookup"><span data-stu-id="85fee-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-from-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85fee-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85fee-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-from-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85fee-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85fee-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-from-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="85fee-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="85fee-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.store]: ../resources/termstore-store.md
[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[Guarde]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "Delete a termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Delete termGroup",
  "suppressions": [
  ]
}
-->
