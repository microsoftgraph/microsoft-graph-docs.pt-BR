---
title: Excluir taskDefinition
description: Excluir uma definição de tarefa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7b576cc5610eb4877a6df65d4da8b819391f7594
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049139"
---
# <a name="delete-taskdefinition"></a><span data-ttu-id="8ebf5-103">Excluir taskDefinition</span><span class="sxs-lookup"><span data-stu-id="8ebf5-103">Delete taskDefinition</span></span>

<span data-ttu-id="8ebf5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ebf5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ebf5-105">Excluir uma **tarefaDefinition**.</span><span class="sxs-lookup"><span data-stu-id="8ebf5-105">Delete a **taskDefinition**.</span></span>

<span data-ttu-id="8ebf5-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="8ebf5-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="8ebf5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ebf5-107">Permissions</span></span>
<span data-ttu-id="8ebf5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ebf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8ebf5-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="8ebf5-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="8ebf5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ebf5-111">Permission type</span></span> | <span data-ttu-id="8ebf5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ebf5-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8ebf5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ebf5-113">Delegated (work or school account)</span></span>| <span data-ttu-id="8ebf5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ebf5-114">Not supported.</span></span> |
|<span data-ttu-id="8ebf5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ebf5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ebf5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ebf5-116">Not Supported.</span></span>|
|<span data-ttu-id="8ebf5-117">Application</span><span class="sxs-lookup"><span data-stu-id="8ebf5-117">Application</span></span>| <span data-ttu-id="8ebf5-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ebf5-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ebf5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ebf5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/taskDefinitions/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8ebf5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ebf5-120">Request headers</span></span>
| <span data-ttu-id="8ebf5-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8ebf5-121">Name</span></span>          | <span data-ttu-id="8ebf5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ebf5-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8ebf5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ebf5-123">Authorization</span></span> | <span data-ttu-id="8ebf5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ebf5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ebf5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ebf5-126">Request body</span></span>
<span data-ttu-id="8ebf5-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ebf5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ebf5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ebf5-128">Response</span></span>
<span data-ttu-id="8ebf5-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ebf5-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ebf5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ebf5-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ebf5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ebf5-132">Request</span></span>
<span data-ttu-id="8ebf5-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ebf5-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8ebf5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ebf5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_taskdefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/taskDefinitions/4c6a0f26-8e5d-4bf6-91e6-4a5731adec19
```
# <a name="c"></a>[<span data-ttu-id="8ebf5-135">C#</span><span class="sxs-lookup"><span data-stu-id="8ebf5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-taskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ebf5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ebf5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-taskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ebf5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ebf5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-taskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8ebf5-138">Java</span><span class="sxs-lookup"><span data-stu-id="8ebf5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-taskdefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="8ebf5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ebf5-139">Response</span></span>
<span data-ttu-id="8ebf5-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8ebf5-140">The following is an example of the response.</span></span>
><span data-ttu-id="8ebf5-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8ebf5-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


