---
title: Listar tarefas
description: Recupere uma lista de tarefas associada a uma definição de tarefa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 5344ce081e53e46e482adc34961a4f4e89bcc4d8
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091537"
---
# <a name="list-tasks"></a><span data-ttu-id="35603-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="35603-103">List tasks</span></span>

<span data-ttu-id="35603-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35603-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35603-105">Recupere uma lista de [tarefas](../resources/printtask.md) associadas a uma [definição de tarefa](../resources/printtaskdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="35603-105">Retrieve a list of [tasks](../resources/printtask.md) associated with a [task definition](../resources/printtaskdefinition.md).</span></span>

<span data-ttu-id="35603-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="35603-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="35603-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="35603-107">Permissions</span></span>
<span data-ttu-id="35603-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35603-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="35603-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="35603-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="35603-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35603-111">Permission type</span></span> | <span data-ttu-id="35603-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35603-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="35603-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35603-113">Delegated (work or school account)</span></span>| <span data-ttu-id="35603-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35603-114">Not supported.</span></span> |
|<span data-ttu-id="35603-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35603-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35603-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35603-116">Not Supported.</span></span>|
|<span data-ttu-id="35603-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35603-117">Application</span></span>| <span data-ttu-id="35603-118">PrintTaskDefinition. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="35603-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="35603-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35603-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}/tasks
```

## <a name="optional-query-parameters"></a><span data-ttu-id="35603-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="35603-120">Optional query parameters</span></span>
<span data-ttu-id="35603-121">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="35603-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="35603-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="35603-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="35603-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="35603-123">Exceptions</span></span>
<span data-ttu-id="35603-124">Não há suporte para alguns operadores: `$count` ,,,, `$format` `$search` `$select` `$skip` , `$top` .</span><span class="sxs-lookup"><span data-stu-id="35603-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35603-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35603-125">Request headers</span></span>
| <span data-ttu-id="35603-126">Nome</span><span class="sxs-lookup"><span data-stu-id="35603-126">Name</span></span>      |<span data-ttu-id="35603-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="35603-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="35603-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="35603-128">Authorization</span></span> | <span data-ttu-id="35603-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35603-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35603-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35603-131">Request body</span></span>
<span data-ttu-id="35603-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="35603-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="35603-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="35603-133">Response</span></span>
<span data-ttu-id="35603-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [multitask](../resources/printtask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35603-134">If successful, this method returns a `200 OK` response code and collection of [printTask](../resources/printtask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="35603-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35603-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="35603-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35603-136">Request</span></span>
<span data-ttu-id="35603-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="35603-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printtaskdefinition_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/92d72a3d-cad7-4809-8924-43833282b079/tasks
```

---

### <a name="response"></a><span data-ttu-id="35603-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="35603-138">Response</span></span>
<span data-ttu-id="35603-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="35603-139">The following is an example of the response.</span></span>
><span data-ttu-id="35603-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35603-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
