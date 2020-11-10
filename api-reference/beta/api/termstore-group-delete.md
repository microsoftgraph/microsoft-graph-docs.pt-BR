---
title: Excluir grupo
description: Excluir um objeto Group.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 7889328e17b68c456737eeca00bb7f21169c5c55
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979918"
---
# <a name="delete-groups"></a><span data-ttu-id="1a838-103">Excluir grupos</span><span class="sxs-lookup"><span data-stu-id="1a838-103">Delete groups</span></span>
<span data-ttu-id="1a838-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="1a838-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a838-105">Excluir um objeto de [grupo](../resources/termstore-group.md) no [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="1a838-105">Delete a [group](../resources/termstore-group.md) object in the term [store].</span></span>

## <a name="permissions"></a><span data-ttu-id="1a838-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a838-106">Permissions</span></span>
<span data-ttu-id="1a838-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a838-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a838-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a838-109">Permission type</span></span>|<span data-ttu-id="1a838-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1a838-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a838-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a838-111">Delegated (work or school account)</span></span> |<span data-ttu-id="1a838-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a838-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="1a838-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a838-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a838-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a838-114">Not supported.</span></span>    |
|<span data-ttu-id="1a838-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a838-115">Application</span></span> | <span data-ttu-id="1a838-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a838-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="1a838-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a838-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/groups/{groupId}
```

## <a name="request-headers"></a><span data-ttu-id="1a838-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a838-118">Request headers</span></span>
|<span data-ttu-id="1a838-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1a838-119">Name</span></span>|<span data-ttu-id="1a838-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a838-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1a838-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a838-121">Authorization</span></span>|<span data-ttu-id="1a838-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a838-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a838-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a838-124">Request body</span></span>
<span data-ttu-id="1a838-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1a838-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a838-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a838-126">Response</span></span>

<span data-ttu-id="1a838-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1a838-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1a838-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1a838-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a838-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a838-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1a838-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a838-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_from_store"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/groups/{groupId}
```
# <a name="c"></a>[<span data-ttu-id="1a838-131">C#</span><span class="sxs-lookup"><span data-stu-id="1a838-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-from-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a838-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a838-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-from-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a838-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a838-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-from-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a838-134">Java</span><span class="sxs-lookup"><span data-stu-id="1a838-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-from-store-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1a838-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a838-135">Response</span></span>
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


