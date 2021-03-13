---
title: Obter tarefa
description: Obter detalhes sobre uma tarefa de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 7b9a9b2e5ff6fdcc3e7bd7c74aa5a173d551f41b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773442"
---
# <a name="get-printtask"></a><span data-ttu-id="f1d07-103">Obter printTask</span><span class="sxs-lookup"><span data-stu-id="f1d07-103">Get printTask</span></span>
<span data-ttu-id="f1d07-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1d07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="f1d07-105">Obter detalhes sobre uma tarefa de impressão.</span><span class="sxs-lookup"><span data-stu-id="f1d07-105">Get details about a print task.</span></span>

<span data-ttu-id="f1d07-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="f1d07-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="f1d07-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1d07-107">Permissions</span></span>
<span data-ttu-id="f1d07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1d07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f1d07-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="f1d07-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="f1d07-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1d07-111">Permission type</span></span> | <span data-ttu-id="f1d07-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1d07-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f1d07-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1d07-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f1d07-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1d07-114">Not supported.</span></span> |
|<span data-ttu-id="f1d07-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1d07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1d07-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1d07-116">Not Supported.</span></span>|
|<span data-ttu-id="f1d07-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1d07-117">Application</span></span>| <span data-ttu-id="f1d07-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1d07-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1d07-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1d07-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="f1d07-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1d07-120">Request headers</span></span>
|<span data-ttu-id="f1d07-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f1d07-121">Name</span></span>|<span data-ttu-id="f1d07-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1d07-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f1d07-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1d07-123">Authorization</span></span>|<span data-ttu-id="f1d07-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1d07-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1d07-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1d07-126">Request body</span></span>
<span data-ttu-id="f1d07-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1d07-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1d07-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1d07-128">Response</span></span>

<span data-ttu-id="f1d07-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printTask](../resources/printtask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1d07-129">If successful, this method returns a `200 OK` response code and a [printTask](../resources/printtask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f1d07-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f1d07-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f1d07-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1d07-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f1d07-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1d07-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printtask"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
```
# <a name="c"></a>[<span data-ttu-id="f1d07-133">C#</span><span class="sxs-lookup"><span data-stu-id="f1d07-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printtask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1d07-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1d07-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printtask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1d07-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1d07-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printtask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f1d07-136">Java</span><span class="sxs-lookup"><span data-stu-id="f1d07-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printtask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f1d07-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1d07-137">Response</span></span>
<span data-ttu-id="f1d07-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f1d07-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

