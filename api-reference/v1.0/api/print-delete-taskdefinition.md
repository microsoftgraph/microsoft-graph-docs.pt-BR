---
title: Excluir taskDefinition
description: Excluir uma definição de tarefa.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: a9f51962e97bad28f3c30048e826c28d60f15455
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777275"
---
# <a name="delete-printtaskdefinition"></a><span data-ttu-id="22501-103">Excluir printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="22501-103">Delete printTaskDefinition</span></span>
<span data-ttu-id="22501-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22501-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="22501-105">Excluir uma **tarefaDefinition**.</span><span class="sxs-lookup"><span data-stu-id="22501-105">Delete a **taskDefinition**.</span></span>

<span data-ttu-id="22501-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="22501-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="22501-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="22501-107">Permissions</span></span>
<span data-ttu-id="22501-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22501-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="22501-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="22501-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="22501-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22501-111">Permission type</span></span> | <span data-ttu-id="22501-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22501-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="22501-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22501-113">Delegated (work or school account)</span></span>| <span data-ttu-id="22501-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22501-114">Not supported.</span></span> |
|<span data-ttu-id="22501-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22501-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22501-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22501-116">Not Supported.</span></span>|
|<span data-ttu-id="22501-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22501-117">Application</span></span>| <span data-ttu-id="22501-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22501-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22501-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22501-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/taskDefinitions/{printTaskDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="22501-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22501-120">Request headers</span></span>
|<span data-ttu-id="22501-121">Nome</span><span class="sxs-lookup"><span data-stu-id="22501-121">Name</span></span>|<span data-ttu-id="22501-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="22501-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="22501-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="22501-123">Authorization</span></span>|<span data-ttu-id="22501-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22501-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22501-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22501-126">Request body</span></span>
<span data-ttu-id="22501-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22501-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22501-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="22501-128">Response</span></span>
<span data-ttu-id="22501-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22501-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22501-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="22501-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="22501-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22501-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="22501-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="22501-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printtaskdefinition"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/taskDefinitions/{printTaskDefinitionId}
```
# <a name="c"></a>[<span data-ttu-id="22501-134">C#</span><span class="sxs-lookup"><span data-stu-id="22501-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printtaskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22501-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22501-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printtaskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22501-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22501-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printtaskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22501-137">Java</span><span class="sxs-lookup"><span data-stu-id="22501-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printtaskdefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="22501-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="22501-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

