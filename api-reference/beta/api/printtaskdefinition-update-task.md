---
title: Atualizar tarefa
description: Atualizar uma tarefa de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d944522ac07e6854b266ea3fb3745d3b95e43525
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035313"
---
# <a name="update-task"></a><span data-ttu-id="07af2-103">Atualizar tarefa</span><span class="sxs-lookup"><span data-stu-id="07af2-103">Update task</span></span>

<span data-ttu-id="07af2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07af2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07af2-105">Atualizar uma tarefa de impressão.</span><span class="sxs-lookup"><span data-stu-id="07af2-105">Update a print task.</span></span>

<span data-ttu-id="07af2-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="07af2-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="07af2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="07af2-107">Permissions</span></span>
<span data-ttu-id="07af2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07af2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="07af2-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="07af2-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="07af2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07af2-111">Permission type</span></span> | <span data-ttu-id="07af2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07af2-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="07af2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07af2-113">Delegated (work or school account)</span></span>| <span data-ttu-id="07af2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07af2-114">Not supported.</span></span> |
|<span data-ttu-id="07af2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07af2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07af2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07af2-116">Not Supported.</span></span>|
|<span data-ttu-id="07af2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07af2-117">Application</span></span>| <span data-ttu-id="07af2-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07af2-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07af2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07af2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/taskDefinitions/{id}/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="07af2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07af2-120">Request headers</span></span>
| <span data-ttu-id="07af2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="07af2-121">Name</span></span>      |<span data-ttu-id="07af2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="07af2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="07af2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="07af2-123">Authorization</span></span> | <span data-ttu-id="07af2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07af2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07af2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07af2-126">Request body</span></span>
<span data-ttu-id="07af2-127">No corpo da solicitação, forneça os valores para os campos de [multitarefa](../resources/printtask.md) relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="07af2-127">In the request body, supply the values for the relevant [printTask](../resources/printtask.md) fields that should be updated.</span></span> <span data-ttu-id="07af2-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="07af2-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="07af2-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="07af2-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="07af2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07af2-130">Property</span></span>     | <span data-ttu-id="07af2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="07af2-131">Type</span></span>        | <span data-ttu-id="07af2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="07af2-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="07af2-133">status</span><span class="sxs-lookup"><span data-stu-id="07af2-133">status</span></span>|<span data-ttu-id="07af2-134">String</span><span class="sxs-lookup"><span data-stu-id="07af2-134">String</span></span>|<span data-ttu-id="07af2-135">Include `state` e `description` valores que descrevem o estado atual da tarefa.</span><span class="sxs-lookup"><span data-stu-id="07af2-135">Include `state` and `description` values that describe the current state of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="07af2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="07af2-136">Response</span></span>
<span data-ttu-id="07af2-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07af2-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="07af2-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07af2-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="07af2-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07af2-140">Request</span></span>
<span data-ttu-id="07af2-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="07af2-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="07af2-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="07af2-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_task"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c/tasks/d036638b-1272-4bba-9227-732463823ed3

{
  "status": {
    "state": "completed",
    "description": "completed"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="07af2-143">C#</span><span class="sxs-lookup"><span data-stu-id="07af2-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07af2-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07af2-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07af2-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07af2-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="07af2-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="07af2-146">Response</span></span>
<span data-ttu-id="07af2-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="07af2-147">The following is an example of the response.</span></span>
><span data-ttu-id="07af2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07af2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update task",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


