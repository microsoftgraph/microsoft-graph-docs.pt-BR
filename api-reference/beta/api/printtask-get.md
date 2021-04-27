---
title: Obter tarefa
description: Obter detalhes sobre uma tarefa de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 06e83c3ca75c0e0e0f2a7fda730456388a43d7bb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053591"
---
# <a name="get-task"></a><span data-ttu-id="f5f57-103">Obter tarefa</span><span class="sxs-lookup"><span data-stu-id="f5f57-103">Get task</span></span>

<span data-ttu-id="f5f57-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5f57-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5f57-105">Obter detalhes sobre uma tarefa de impressão.</span><span class="sxs-lookup"><span data-stu-id="f5f57-105">Get details about a print task.</span></span>

<span data-ttu-id="f5f57-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="f5f57-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="f5f57-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5f57-107">Permissions</span></span>
<span data-ttu-id="f5f57-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5f57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f5f57-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="f5f57-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="f5f57-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5f57-111">Permission type</span></span> | <span data-ttu-id="f5f57-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5f57-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f5f57-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5f57-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f5f57-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5f57-114">Not supported.</span></span> |
|<span data-ttu-id="f5f57-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5f57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5f57-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5f57-116">Not Supported.</span></span>|
|<span data-ttu-id="f5f57-117">Application</span><span class="sxs-lookup"><span data-stu-id="f5f57-117">Application</span></span>| <span data-ttu-id="f5f57-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5f57-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5f57-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5f57-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f5f57-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f57-120">Request headers</span></span>
| <span data-ttu-id="f5f57-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f5f57-121">Name</span></span>      |<span data-ttu-id="f5f57-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5f57-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f5f57-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5f57-123">Authorization</span></span> | <span data-ttu-id="f5f57-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5f57-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5f57-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f57-126">Request body</span></span>
<span data-ttu-id="f5f57-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5f57-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f5f57-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f57-128">Response</span></span>
<span data-ttu-id="f5f57-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printTask](../resources/printtask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5f57-129">If successful, this method returns a `200 OK` response code and a [printTask](../resources/printtask.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5f57-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5f57-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="f5f57-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f57-131">Request</span></span>
<span data-ttu-id="f5f57-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5f57-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f5f57-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5f57-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_task"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c/tasks/d036638b-1272-4bba-9227-732463823ed3
```
# <a name="c"></a>[<span data-ttu-id="f5f57-134">C#</span><span class="sxs-lookup"><span data-stu-id="f5f57-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5f57-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5f57-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5f57-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5f57-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5f57-137">Java</span><span class="sxs-lookup"><span data-stu-id="f5f57-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-task-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="f5f57-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f57-138">Response</span></span>
<span data-ttu-id="f5f57-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f5f57-139">The following is an example of the response.</span></span>
><span data-ttu-id="f5f57-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f5f57-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 392

{

  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions('3203656e-6069-4e10-8147-d25290b00a3c')/tasks/$entity",
  "id": "d036638b-1272-4bba-9227-732463823ed3",
  "parentUrl": "https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
  "status": {
    "state": "completed",
    "description": "completed"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get task",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


