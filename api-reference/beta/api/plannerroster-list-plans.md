---
title: Listar planos
description: Obter os recursos plannerPlan da propriedade de navegação de planos.
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: b3dc12e051c7d301cef1ec9e361ae5620fc5410f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961546"
---
# <a name="list-plans"></a><span data-ttu-id="bd9fe-103">Listar planos</span><span class="sxs-lookup"><span data-stu-id="bd9fe-103">List plans</span></span>
<span data-ttu-id="bd9fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd9fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd9fe-105">Obter os [plannerPlans contidos](../resources/plannerplan.md) pelo [plannerRoster](../resources/plannerRoster.md).</span><span class="sxs-lookup"><span data-stu-id="bd9fe-105">Get the [plannerPlans](../resources/plannerplan.md) contained by the [plannerRoster](../resources/plannerRoster.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bd9fe-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd9fe-106">Permissions</span></span>
<span data-ttu-id="bd9fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd9fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd9fe-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd9fe-109">Permission type</span></span>|<span data-ttu-id="bd9fe-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd9fe-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd9fe-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd9fe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bd9fe-112">Tasks.Read, Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd9fe-112">Tasks.Read, Tasks.ReadWrite</span></span>|
|<span data-ttu-id="bd9fe-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd9fe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd9fe-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd9fe-114">Not supported.</span></span>|
|<span data-ttu-id="bd9fe-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd9fe-115">Application</span></span>|<span data-ttu-id="bd9fe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd9fe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd9fe-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd9fe-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /planner/rosters/{plannerRosterId}/plans
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd9fe-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bd9fe-118">Optional query parameters</span></span>
<span data-ttu-id="bd9fe-119">Este método só dá suporte a seguintes parâmetros de consulta OData:</span><span class="sxs-lookup"><span data-stu-id="bd9fe-119">This method only supports following OData query parameters:</span></span>

- <span data-ttu-id="bd9fe-120">$select</span><span class="sxs-lookup"><span data-stu-id="bd9fe-120">$select</span></span>

<span data-ttu-id="bd9fe-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bd9fe-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd9fe-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd9fe-122">Request headers</span></span>
|<span data-ttu-id="bd9fe-123">Nome</span><span class="sxs-lookup"><span data-stu-id="bd9fe-123">Name</span></span>|<span data-ttu-id="bd9fe-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd9fe-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bd9fe-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd9fe-125">Authorization</span></span>|<span data-ttu-id="bd9fe-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd9fe-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd9fe-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd9fe-128">Request body</span></span>
<span data-ttu-id="bd9fe-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd9fe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd9fe-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd9fe-130">Response</span></span>

<span data-ttu-id="bd9fe-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd9fe-131">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd9fe-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bd9fe-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd9fe-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd9fe-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bd9fe-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd9fe-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_plannerplan_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/planner/rosters/6519868f-868f-6519-8f86-19658f861965/plans
```
# <a name="c"></a>[<span data-ttu-id="bd9fe-135">C#</span><span class="sxs-lookup"><span data-stu-id="bd9fe-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-plannerplan-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd9fe-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd9fe-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-plannerplan-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd9fe-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd9fe-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-plannerplan-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd9fe-138">Java</span><span class="sxs-lookup"><span data-stu-id="bd9fe-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-plannerplan-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="bd9fe-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd9fe-139">Response</span></span>
<span data-ttu-id="bd9fe-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bd9fe-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.plannerPlan)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.plannerPlan",
      "id": "c6442b38-2b38-c644-382b-44c6382b44c6",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "title": "Test plan",
      "container": {
        "@odata.type": "microsoft.graph.plannerPlanContainer",
        "url": "https://graph.microsoft.com/beta/planner/rosters/6519868f-868f-6519-8f86-19658f861965",
        "containerId": "6519868f-868f-6519-8f86-19658f861965",
        "type": "roster"
      }
    }
  ]
}
```

