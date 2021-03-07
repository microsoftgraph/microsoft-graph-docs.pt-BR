---
title: Listar tarefas
description: Recupere uma lista de tarefas associada a uma definição de tarefa.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 21bfb3aa732319531c084547d50593d77131af04
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516894"
---
# <a name="list-tasks"></a><span data-ttu-id="0bc62-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="0bc62-103">List tasks</span></span>
<span data-ttu-id="0bc62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bc62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="0bc62-105">Recupere uma lista de [tarefas](../resources/printtask.md) associadas a uma [definição de tarefa](../resources/printtaskdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0bc62-105">Retrieve a list of [tasks](../resources/printtask.md) associated with a [task definition](../resources/printtaskdefinition.md).</span></span>

<span data-ttu-id="0bc62-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="0bc62-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="0bc62-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0bc62-107">Permissions</span></span>
<span data-ttu-id="0bc62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bc62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0bc62-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="0bc62-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="0bc62-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0bc62-111">Permission type</span></span> | <span data-ttu-id="0bc62-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0bc62-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0bc62-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0bc62-113">Delegated (work or school account)</span></span>| <span data-ttu-id="0bc62-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bc62-114">Not supported.</span></span> |
|<span data-ttu-id="0bc62-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0bc62-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bc62-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bc62-116">Not Supported.</span></span>|
|<span data-ttu-id="0bc62-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bc62-117">Application</span></span>| <span data-ttu-id="0bc62-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bc62-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bc62-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0bc62-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/taskDefinitions/{taskDefinitionId}/tasks
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0bc62-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0bc62-120">Optional query parameters</span></span>
<span data-ttu-id="0bc62-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0bc62-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0bc62-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0bc62-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="0bc62-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="0bc62-123">Exceptions</span></span>
<span data-ttu-id="0bc62-124">Alguns operadores não têm suporte: `$count` , , , , , , `$format` `$search` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="0bc62-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0bc62-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0bc62-125">Request headers</span></span>
|<span data-ttu-id="0bc62-126">Nome</span><span class="sxs-lookup"><span data-stu-id="0bc62-126">Name</span></span>|<span data-ttu-id="0bc62-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bc62-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0bc62-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="0bc62-128">Authorization</span></span>|<span data-ttu-id="0bc62-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bc62-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bc62-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0bc62-131">Request body</span></span>
<span data-ttu-id="0bc62-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0bc62-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bc62-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bc62-133">Response</span></span>

<span data-ttu-id="0bc62-134">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos printTask](../resources/printtask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bc62-134">If successful, this method returns a `200 OK` response code and a collection of [printTask](../resources/printtask.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0bc62-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0bc62-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0bc62-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bc62-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printtask"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}/tasks
```

### <a name="response"></a><span data-ttu-id="0bc62-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bc62-137">Response</span></span>
<span data-ttu-id="0bc62-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0bc62-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printTask)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.printTask)",
  "value": [
    {
      "id": "d036638b-1272-4bba-9227-732463823ed3",
      "parentUrl": "https://graph.microsoft.com/v1.0/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
      "status": {
        "state": "processing",
        "description": "The task is being processed."
      }
    }
  ]
}
```

