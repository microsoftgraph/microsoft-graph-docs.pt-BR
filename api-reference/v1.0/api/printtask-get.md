---
title: Obter tarefa
description: Obter detalhes sobre uma tarefa de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 0aff8e70271a0903289a50eb4fb76b21d9269cab
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516847"
---
# <a name="get-printtask"></a><span data-ttu-id="2e15f-103">Obter printTask</span><span class="sxs-lookup"><span data-stu-id="2e15f-103">Get printTask</span></span>
<span data-ttu-id="2e15f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e15f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="2e15f-105">Obter detalhes sobre uma tarefa de impressão.</span><span class="sxs-lookup"><span data-stu-id="2e15f-105">Get details about a print task.</span></span>

<span data-ttu-id="2e15f-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="2e15f-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="2e15f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e15f-107">Permissions</span></span>
<span data-ttu-id="2e15f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e15f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2e15f-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="2e15f-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="2e15f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e15f-111">Permission type</span></span> | <span data-ttu-id="2e15f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e15f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2e15f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e15f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="2e15f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e15f-114">Not supported.</span></span> |
|<span data-ttu-id="2e15f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e15f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e15f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e15f-116">Not Supported.</span></span>|
|<span data-ttu-id="2e15f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e15f-117">Application</span></span>| <span data-ttu-id="2e15f-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e15f-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e15f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e15f-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="2e15f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e15f-120">Request headers</span></span>
|<span data-ttu-id="2e15f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2e15f-121">Name</span></span>|<span data-ttu-id="2e15f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e15f-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2e15f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e15f-123">Authorization</span></span>|<span data-ttu-id="2e15f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e15f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e15f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e15f-126">Request body</span></span>
<span data-ttu-id="2e15f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e15f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e15f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e15f-128">Response</span></span>

<span data-ttu-id="2e15f-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printTask](../resources/printtask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e15f-129">If successful, this method returns a `200 OK` response code and a [printTask](../resources/printtask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e15f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2e15f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e15f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e15f-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printtask"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
```

### <a name="response"></a><span data-ttu-id="2e15f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e15f-132">Response</span></span>
<span data-ttu-id="2e15f-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2e15f-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/taskDefinitions('3203656e-6069-4e10-8147-d25290b00a3c')/tasks/$entity",
  "id": "d036638b-1272-4bba-9227-732463823ed3",
  "parentUrl": "https://graph.microsoft.com/v1.0/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
  "status": {
    "state": "completed",
    "description": "completed"
  }
}
```

