---
title: Atualizar tarefa
description: Atualizar uma tarefa de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 684d2063f069b3e7444e0727c2b2d9ad14fe7113
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517022"
---
# <a name="update-printtask"></a><span data-ttu-id="c41d5-103">Atualizar printTask</span><span class="sxs-lookup"><span data-stu-id="c41d5-103">Update printTask</span></span>
<span data-ttu-id="c41d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c41d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="c41d5-105">Atualizar uma tarefa de impressão.</span><span class="sxs-lookup"><span data-stu-id="c41d5-105">Update a print task.</span></span>

<span data-ttu-id="c41d5-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="c41d5-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="c41d5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c41d5-107">Permissions</span></span>
<span data-ttu-id="c41d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c41d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c41d5-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="c41d5-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="c41d5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c41d5-111">Permission type</span></span> | <span data-ttu-id="c41d5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c41d5-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c41d5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c41d5-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c41d5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c41d5-114">Not supported.</span></span> |
|<span data-ttu-id="c41d5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c41d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c41d5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c41d5-116">Not Supported.</span></span>|
|<span data-ttu-id="c41d5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c41d5-117">Application</span></span>| <span data-ttu-id="c41d5-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c41d5-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c41d5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c41d5-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="c41d5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c41d5-120">Request headers</span></span>
|<span data-ttu-id="c41d5-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c41d5-121">Name</span></span>|<span data-ttu-id="c41d5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c41d5-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c41d5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c41d5-123">Authorization</span></span>|<span data-ttu-id="c41d5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c41d5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c41d5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c41d5-126">Content-Type</span></span>|<span data-ttu-id="c41d5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c41d5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c41d5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c41d5-129">Request body</span></span>

<span data-ttu-id="c41d5-130">No corpo da solicitação, fornece os valores dos campos [printTask relevantes](../resources/printtask.md) que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="c41d5-130">In the request body, supply the values for the relevant [printTask](../resources/printtask.md) fields that should be updated.</span></span> <span data-ttu-id="c41d5-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="c41d5-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c41d5-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c41d5-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c41d5-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c41d5-133">Property</span></span>     | <span data-ttu-id="c41d5-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="c41d5-134">Type</span></span>        | <span data-ttu-id="c41d5-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="c41d5-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c41d5-136">status</span><span class="sxs-lookup"><span data-stu-id="c41d5-136">status</span></span>|<span data-ttu-id="c41d5-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c41d5-137">String</span></span>|<span data-ttu-id="c41d5-138">Inclua `state` e valores que descrevem o estado atual da `description` tarefa.</span><span class="sxs-lookup"><span data-stu-id="c41d5-138">Include `state` and `description` values that describe the current state of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="c41d5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c41d5-139">Response</span></span>

<span data-ttu-id="c41d5-140">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printTask](../resources/printtask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c41d5-140">If successful, this method returns a `200 OK` response code and an updated [printTask](../resources/printtask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c41d5-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c41d5-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c41d5-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c41d5-142">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="c41d5-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c41d5-143">Response</span></span>
<span data-ttu-id="c41d5-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c41d5-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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

