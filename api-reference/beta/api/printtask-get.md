---
title: Obter tarefa
description: Obter detalhes sobre uma tarefa de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: f8383716aca2a4dc0e4314bd62b5af43037fffd9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035328"
---
# <a name="get-task"></a><span data-ttu-id="56ac8-103">Obter tarefa</span><span class="sxs-lookup"><span data-stu-id="56ac8-103">Get task</span></span>

<span data-ttu-id="56ac8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56ac8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56ac8-105">Obter detalhes sobre uma tarefa de impressão.</span><span class="sxs-lookup"><span data-stu-id="56ac8-105">Get details about a print task.</span></span>

<span data-ttu-id="56ac8-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="56ac8-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="56ac8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="56ac8-107">Permissions</span></span>
<span data-ttu-id="56ac8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56ac8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="56ac8-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="56ac8-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="56ac8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56ac8-111">Permission type</span></span> | <span data-ttu-id="56ac8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56ac8-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="56ac8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56ac8-113">Delegated (work or school account)</span></span>| <span data-ttu-id="56ac8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56ac8-114">Not supported.</span></span> |
|<span data-ttu-id="56ac8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56ac8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56ac8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56ac8-116">Not Supported.</span></span>|
|<span data-ttu-id="56ac8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56ac8-117">Application</span></span>| <span data-ttu-id="56ac8-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56ac8-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56ac8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56ac8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="56ac8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56ac8-120">Request headers</span></span>
| <span data-ttu-id="56ac8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="56ac8-121">Name</span></span>      |<span data-ttu-id="56ac8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="56ac8-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="56ac8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="56ac8-123">Authorization</span></span> | <span data-ttu-id="56ac8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56ac8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56ac8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56ac8-126">Request body</span></span>
<span data-ttu-id="56ac8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="56ac8-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="56ac8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="56ac8-128">Response</span></span>
<span data-ttu-id="56ac8-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [multitask](../resources/printtask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56ac8-129">If successful, this method returns a `200 OK` response code and a [printTask](../resources/printtask.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56ac8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56ac8-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="56ac8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56ac8-131">Request</span></span>
<span data-ttu-id="56ac8-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="56ac8-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="56ac8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="56ac8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_task"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c/tasks/d036638b-1272-4bba-9227-732463823ed3
```
# <a name="c"></a>[<span data-ttu-id="56ac8-134">C#</span><span class="sxs-lookup"><span data-stu-id="56ac8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56ac8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56ac8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56ac8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56ac8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="56ac8-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="56ac8-137">Response</span></span>
<span data-ttu-id="56ac8-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="56ac8-138">The following is an example of the response.</span></span>
><span data-ttu-id="56ac8-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56ac8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


