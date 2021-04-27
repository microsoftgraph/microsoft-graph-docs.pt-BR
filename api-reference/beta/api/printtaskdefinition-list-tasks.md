---
title: Listar tarefas
description: Recupere uma lista de tarefas associada a uma definição de tarefa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: e489a7a1c34a60d1f1da45d151a50e46511e6ca0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053577"
---
# <a name="list-tasks"></a><span data-ttu-id="8c9e0-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="8c9e0-103">List tasks</span></span>

<span data-ttu-id="8c9e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c9e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c9e0-105">Recupere uma lista de [tarefas](../resources/printtask.md) associadas a uma [definição de tarefa](../resources/printtaskdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8c9e0-105">Retrieve a list of [tasks](../resources/printtask.md) associated with a [task definition](../resources/printtaskdefinition.md).</span></span>

<span data-ttu-id="8c9e0-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="8c9e0-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c9e0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c9e0-107">Permissions</span></span>
<span data-ttu-id="8c9e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c9e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8c9e0-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="8c9e0-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="8c9e0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c9e0-111">Permission type</span></span> | <span data-ttu-id="8c9e0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c9e0-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8c9e0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c9e0-113">Delegated (work or school account)</span></span>| <span data-ttu-id="8c9e0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c9e0-114">Not supported.</span></span> |
|<span data-ttu-id="8c9e0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c9e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c9e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c9e0-116">Not Supported.</span></span>|
|<span data-ttu-id="8c9e0-117">Application</span><span class="sxs-lookup"><span data-stu-id="8c9e0-117">Application</span></span>| <span data-ttu-id="8c9e0-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c9e0-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c9e0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c9e0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}/tasks
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c9e0-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8c9e0-120">Optional query parameters</span></span>
<span data-ttu-id="8c9e0-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8c9e0-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8c9e0-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8c9e0-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="8c9e0-123">Exceções</span><span class="sxs-lookup"><span data-stu-id="8c9e0-123">Exceptions</span></span>
<span data-ttu-id="8c9e0-124">Alguns operadores não têm suporte: `$count` , , , , , , `$format` `$search` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="8c9e0-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c9e0-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c9e0-125">Request headers</span></span>
| <span data-ttu-id="8c9e0-126">Nome</span><span class="sxs-lookup"><span data-stu-id="8c9e0-126">Name</span></span>      |<span data-ttu-id="8c9e0-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c9e0-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c9e0-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c9e0-128">Authorization</span></span> | <span data-ttu-id="8c9e0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c9e0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c9e0-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c9e0-131">Request body</span></span>
<span data-ttu-id="8c9e0-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8c9e0-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8c9e0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c9e0-133">Response</span></span>
<span data-ttu-id="8c9e0-134">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [printTask](../resources/printtask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c9e0-134">If successful, this method returns a `200 OK` response code and collection of [printTask](../resources/printtask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8c9e0-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c9e0-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c9e0-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c9e0-136">Request</span></span>
<span data-ttu-id="8c9e0-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c9e0-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8c9e0-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c9e0-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printtaskdefinition_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/92d72a3d-cad7-4809-8924-43833282b079/tasks
```
# <a name="c"></a>[<span data-ttu-id="8c9e0-139">C#</span><span class="sxs-lookup"><span data-stu-id="8c9e0-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printtaskdefinition-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c9e0-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c9e0-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printtaskdefinition-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c9e0-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c9e0-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printtaskdefinition-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c9e0-142">Java</span><span class="sxs-lookup"><span data-stu-id="8c9e0-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printtaskdefinition-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="8c9e0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c9e0-143">Response</span></span>
<span data-ttu-id="8c9e0-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8c9e0-144">The following is an example of the response.</span></span>
><span data-ttu-id="8c9e0-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8c9e0-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 429

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printTask)",
  "value": [
    {
      "id": "d036638b-1272-4bba-9227-732463823ed3",
      "parentUrl": "https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
      "status": {
        "state": "processing",
        "description": "The task is being processed."
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


