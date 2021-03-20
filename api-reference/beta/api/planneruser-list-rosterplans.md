---
title: Listar rosterPlans
description: Obter os recursos plannerPlan da propriedade de navegação rosterPlans.
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 68b62d68620f205f3933f7a876746e19ab8f3e0c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953215"
---
# <a name="list-rosterplans"></a><span data-ttu-id="d3395-103">Listar rosterPlans</span><span class="sxs-lookup"><span data-stu-id="d3395-103">List rosterPlans</span></span>
<span data-ttu-id="d3395-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3395-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3395-105">Obter a lista de [plannerPlans](../resources/plannerplan.md) contidos pelos [plannerRosters](../resources/plannerroster.md) dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="d3395-105">Get the list of [plannerPlans](../resources/plannerplan.md) that are contained by the [plannerRosters](../resources/plannerroster.md) of which the user is a member.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3395-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3395-106">Permissions</span></span>
<span data-ttu-id="d3395-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3395-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3395-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3395-109">Permission type</span></span>|<span data-ttu-id="d3395-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3395-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3395-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3395-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d3395-112">Tasks.Read, Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3395-112">Tasks.Read, Tasks.ReadWrite</span></span>|
|<span data-ttu-id="d3395-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3395-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3395-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3395-114">Not supported.</span></span>|
|<span data-ttu-id="d3395-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3395-115">Application</span></span>|<span data-ttu-id="d3395-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3395-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3395-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3395-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/planner/rosterPlans
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3395-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d3395-118">Optional query parameters</span></span>
<span data-ttu-id="d3395-119">Este método só dá suporte a seguintes parâmetros de consulta OData:</span><span class="sxs-lookup"><span data-stu-id="d3395-119">This method only supports following OData query parameters:</span></span>

- <span data-ttu-id="d3395-120">$select</span><span class="sxs-lookup"><span data-stu-id="d3395-120">$select</span></span>

<span data-ttu-id="d3395-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d3395-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3395-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3395-122">Request headers</span></span>
|<span data-ttu-id="d3395-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d3395-123">Name</span></span>|<span data-ttu-id="d3395-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3395-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d3395-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3395-125">Authorization</span></span>|<span data-ttu-id="d3395-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3395-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3395-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3395-128">Request body</span></span>
<span data-ttu-id="d3395-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3395-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3395-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3395-130">Response</span></span>

<span data-ttu-id="d3395-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3395-131">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3395-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d3395-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3395-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3395-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d3395-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3395-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_plannerplan_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/planner/rosterPlans
```
# <a name="c"></a>[<span data-ttu-id="d3395-135">C#</span><span class="sxs-lookup"><span data-stu-id="d3395-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-plannerplan-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3395-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3395-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-plannerplan-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3395-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3395-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-plannerplan-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3395-138">Java</span><span class="sxs-lookup"><span data-stu-id="d3395-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-plannerplan-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d3395-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3395-139">Response</span></span>
<span data-ttu-id="d3395-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d3395-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
        "url": "https://graph.microsoft.com/beta/planner/rosters/5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38",
        "containerId": "5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38",
        "type": "roster"
      }
    }
  ]
}
```

