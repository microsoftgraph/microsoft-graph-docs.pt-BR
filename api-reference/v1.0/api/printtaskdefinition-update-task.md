---
title: Atualizar tarefa
description: Atualizar uma tarefa de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 1375b48ccecc800111b0e84065f58324124021d4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771292"
---
# <a name="update-printtask"></a><span data-ttu-id="32069-103">Atualizar printTask</span><span class="sxs-lookup"><span data-stu-id="32069-103">Update printTask</span></span>
<span data-ttu-id="32069-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32069-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="32069-105">Atualizar uma tarefa de impressão.</span><span class="sxs-lookup"><span data-stu-id="32069-105">Update a print task.</span></span>

<span data-ttu-id="32069-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="32069-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="32069-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="32069-107">Permissions</span></span>
<span data-ttu-id="32069-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32069-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="32069-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="32069-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="32069-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32069-111">Permission type</span></span> | <span data-ttu-id="32069-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32069-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="32069-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32069-113">Delegated (work or school account)</span></span>| <span data-ttu-id="32069-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32069-114">Not supported.</span></span> |
|<span data-ttu-id="32069-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32069-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32069-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32069-116">Not Supported.</span></span>|
|<span data-ttu-id="32069-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32069-117">Application</span></span>| <span data-ttu-id="32069-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32069-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32069-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32069-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="32069-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32069-120">Request headers</span></span>
|<span data-ttu-id="32069-121">Nome</span><span class="sxs-lookup"><span data-stu-id="32069-121">Name</span></span>|<span data-ttu-id="32069-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="32069-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="32069-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="32069-123">Authorization</span></span>|<span data-ttu-id="32069-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32069-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="32069-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32069-126">Content-Type</span></span>|<span data-ttu-id="32069-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32069-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32069-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32069-129">Request body</span></span>

<span data-ttu-id="32069-130">No corpo da solicitação, fornece os valores dos campos [printTask relevantes](../resources/printtask.md) que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="32069-130">In the request body, supply the values for the relevant [printTask](../resources/printtask.md) fields that should be updated.</span></span> <span data-ttu-id="32069-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="32069-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="32069-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="32069-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="32069-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32069-133">Property</span></span>     | <span data-ttu-id="32069-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="32069-134">Type</span></span>        | <span data-ttu-id="32069-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="32069-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="32069-136">status</span><span class="sxs-lookup"><span data-stu-id="32069-136">status</span></span>|<span data-ttu-id="32069-137">String</span><span class="sxs-lookup"><span data-stu-id="32069-137">String</span></span>|<span data-ttu-id="32069-138">Inclua `state` e valores que descrevem o estado atual da `description` tarefa.</span><span class="sxs-lookup"><span data-stu-id="32069-138">Include `state` and `description` values that describe the current state of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="32069-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="32069-139">Response</span></span>

<span data-ttu-id="32069-140">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printTask](../resources/printtask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32069-140">If successful, this method returns a `200 OK` response code and an updated [printTask](../resources/printtask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="32069-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="32069-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="32069-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32069-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="32069-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="32069-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printtask"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
Content-Type: application/json
Content-length: 152

{
  "status": {
    "state": "completed",
    "description": "completed"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="32069-144">C#</span><span class="sxs-lookup"><span data-stu-id="32069-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printtask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32069-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32069-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printtask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32069-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32069-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printtask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32069-147">Java</span><span class="sxs-lookup"><span data-stu-id="32069-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printtask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="32069-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="32069-148">Response</span></span>
<span data-ttu-id="32069-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="32069-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTask"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "d036638b-1272-4bba-9227-732463823ed3",
  "parentUrl": "https://graph.microsoft.com/v1.0/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
  "status": {
    "state": "completed",
    "description": "Task execution is completed."
  }
}
```

