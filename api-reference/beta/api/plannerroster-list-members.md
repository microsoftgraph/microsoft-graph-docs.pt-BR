---
title: Listar membros de uma lista de participantes
description: Obter os recursos plannerRosterMember da propriedade de navegação members.
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 9c08f29581b549014544ed1de43f6562efb5066f
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272532"
---
# <a name="list-members-of-a-roster"></a><span data-ttu-id="26954-103">Listar membros de uma lista de participantes</span><span class="sxs-lookup"><span data-stu-id="26954-103">List members of a roster</span></span>
<span data-ttu-id="26954-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26954-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26954-105">Obter a lista de [plannerRosterMembers](../resources/plannerrostermember.md) de um [plannerRoster](../resources/plannerroster.md).</span><span class="sxs-lookup"><span data-stu-id="26954-105">Get the list of [plannerRosterMembers](../resources/plannerrostermember.md) from a [plannerRoster](../resources/plannerroster.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="26954-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="26954-106">Permissions</span></span>
<span data-ttu-id="26954-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26954-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26954-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26954-109">Permission type</span></span>|<span data-ttu-id="26954-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26954-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26954-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26954-111">Delegated (work or school account)</span></span>|<span data-ttu-id="26954-112">Tasks.Read, Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26954-112">Tasks.Read, Tasks.ReadWrite</span></span>|
|<span data-ttu-id="26954-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26954-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26954-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26954-114">Not supported.</span></span>|
|<span data-ttu-id="26954-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26954-115">Application</span></span>|<span data-ttu-id="26954-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26954-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26954-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26954-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /planner/rosters/{plannerRosterId}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="26954-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="26954-118">Optional query parameters</span></span>
<span data-ttu-id="26954-119">Esse método só dá suporte aos seguintes parâmetros de consulta OData:</span><span class="sxs-lookup"><span data-stu-id="26954-119">This method only supports following OData query parameters:</span></span>

- <span data-ttu-id="26954-120">$select</span><span class="sxs-lookup"><span data-stu-id="26954-120">$select</span></span>

<span data-ttu-id="26954-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="26954-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="26954-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26954-122">Request headers</span></span>
|<span data-ttu-id="26954-123">Nome</span><span class="sxs-lookup"><span data-stu-id="26954-123">Name</span></span>|<span data-ttu-id="26954-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="26954-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="26954-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="26954-125">Authorization</span></span>|<span data-ttu-id="26954-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26954-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26954-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26954-128">Request body</span></span>
<span data-ttu-id="26954-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="26954-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26954-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="26954-130">Response</span></span>

<span data-ttu-id="26954-131">Se bem-sucedido, este método retorna um código de resposta e uma coleção de objetos `200 OK` [plannerRosterMember](../resources/plannerrostermember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26954-131">If successful, this method returns a `200 OK` response code and a collection of [plannerRosterMember](../resources/plannerrostermember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26954-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="26954-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26954-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26954-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="26954-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="26954-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_plannerrostermember"
}
-->
``` http
GET https://graph.microsoft.com/beta/planner/rosters/6519868f-868f-6519-8f86-19658f861965/members
```
# <a name="c"></a>[<span data-ttu-id="26954-135">C#</span><span class="sxs-lookup"><span data-stu-id="26954-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-plannerrostermember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26954-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26954-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-plannerrostermember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26954-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26954-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-plannerrostermember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26954-138">Java</span><span class="sxs-lookup"><span data-stu-id="26954-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-plannerrostermember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="26954-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="26954-139">Response</span></span>
<span data-ttu-id="26954-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="26954-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.plannerRosterMember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.plannerRosterMember",
      "id": "670095cd-95cd-6700-cd95-0067cd950067",
      "userId": "5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38",
      "tenantId": "7084c257-c1b7-4286-98b0-20ea7b5c1319",
      "roles": [
      ]
    }
  ]
}
```

