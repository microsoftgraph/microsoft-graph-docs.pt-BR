---
title: Atualizar tarefa
description: Atualizar uma tarefa de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 33c6078aa9265788409abd3e23d736fab9989b0b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053570"
---
# <a name="update-task"></a><span data-ttu-id="09d41-103">Atualizar tarefa</span><span class="sxs-lookup"><span data-stu-id="09d41-103">Update task</span></span>

<span data-ttu-id="09d41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09d41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09d41-105">Atualizar uma tarefa de impressão.</span><span class="sxs-lookup"><span data-stu-id="09d41-105">Update a print task.</span></span>

<span data-ttu-id="09d41-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="09d41-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="09d41-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="09d41-107">Permissions</span></span>
<span data-ttu-id="09d41-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09d41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="09d41-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="09d41-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="09d41-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09d41-111">Permission type</span></span> | <span data-ttu-id="09d41-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09d41-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="09d41-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09d41-113">Delegated (work or school account)</span></span>| <span data-ttu-id="09d41-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09d41-114">Not supported.</span></span> |
|<span data-ttu-id="09d41-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09d41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09d41-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09d41-116">Not Supported.</span></span>|
|<span data-ttu-id="09d41-117">Application</span><span class="sxs-lookup"><span data-stu-id="09d41-117">Application</span></span>| <span data-ttu-id="09d41-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09d41-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09d41-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09d41-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/taskDefinitions/{id}/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="09d41-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09d41-120">Request headers</span></span>
| <span data-ttu-id="09d41-121">Nome</span><span class="sxs-lookup"><span data-stu-id="09d41-121">Name</span></span>      |<span data-ttu-id="09d41-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="09d41-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="09d41-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="09d41-123">Authorization</span></span> | <span data-ttu-id="09d41-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09d41-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09d41-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09d41-126">Request body</span></span>
<span data-ttu-id="09d41-127">No corpo da solicitação, fornece os valores dos campos [printTask relevantes](../resources/printtask.md) que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="09d41-127">In the request body, supply the values for the relevant [printTask](../resources/printtask.md) fields that should be updated.</span></span> <span data-ttu-id="09d41-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="09d41-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="09d41-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="09d41-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="09d41-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09d41-130">Property</span></span>     | <span data-ttu-id="09d41-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="09d41-131">Type</span></span>        | <span data-ttu-id="09d41-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="09d41-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="09d41-133">status</span><span class="sxs-lookup"><span data-stu-id="09d41-133">status</span></span>|<span data-ttu-id="09d41-134">String</span><span class="sxs-lookup"><span data-stu-id="09d41-134">String</span></span>|<span data-ttu-id="09d41-135">Inclua `state` e valores que descrevem o estado atual da `description` tarefa.</span><span class="sxs-lookup"><span data-stu-id="09d41-135">Include `state` and `description` values that describe the current state of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="09d41-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="09d41-136">Response</span></span>
<span data-ttu-id="09d41-137">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printTask](../resources/printtask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09d41-137">If successful, this method returns a `200 OK` response code and an updated [printTask](../resources/printtask.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="09d41-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09d41-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="09d41-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09d41-139">Request</span></span>
<span data-ttu-id="09d41-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="09d41-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="09d41-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="09d41-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="09d41-142">C#</span><span class="sxs-lookup"><span data-stu-id="09d41-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09d41-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09d41-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09d41-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09d41-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="09d41-145">Java</span><span class="sxs-lookup"><span data-stu-id="09d41-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-task-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="09d41-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="09d41-146">Response</span></span>
<span data-ttu-id="09d41-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="09d41-147">The following is an example of the response.</span></span>
><span data-ttu-id="09d41-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="09d41-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTask"
}
-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "d036638b-1272-4bba-9227-732463823ed3",
  "parentUrl": "https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
  "status": {
    "state": "completed",
    "description": "Task execution is completed."
  }
}
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


