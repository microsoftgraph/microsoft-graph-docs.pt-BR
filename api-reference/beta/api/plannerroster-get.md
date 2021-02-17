---
title: Obter plannerRoster
description: Leia as propriedades e os relacionamentos de um objeto plannerRoster.
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 49aa19c85cea3d103b6338a46ccd605c89759e95
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271880"
---
# <a name="get-plannerroster"></a><span data-ttu-id="21fd1-103">Obter plannerRoster</span><span class="sxs-lookup"><span data-stu-id="21fd1-103">Get plannerRoster</span></span>
<span data-ttu-id="21fd1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21fd1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21fd1-105">Leia as propriedades e os relacionamentos de um [objeto plannerRoster.](../resources/plannerroster.md)</span><span class="sxs-lookup"><span data-stu-id="21fd1-105">Read the properties and relationships of a [plannerRoster](../resources/plannerroster.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="21fd1-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="21fd1-106">Permissions</span></span>
<span data-ttu-id="21fd1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21fd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21fd1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21fd1-109">Permission type</span></span>|<span data-ttu-id="21fd1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21fd1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21fd1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21fd1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="21fd1-112">Tasks.Read, Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21fd1-112">Tasks.Read, Tasks.ReadWrite</span></span>|
|<span data-ttu-id="21fd1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21fd1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21fd1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21fd1-114">Not supported.</span></span>|
|<span data-ttu-id="21fd1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21fd1-115">Application</span></span>|<span data-ttu-id="21fd1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21fd1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21fd1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21fd1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /planner/rosters/{plannerRosterId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21fd1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="21fd1-118">Optional query parameters</span></span>
<span data-ttu-id="21fd1-119">Esse método só dá suporte aos seguintes parâmetros de consulta OData:</span><span class="sxs-lookup"><span data-stu-id="21fd1-119">This method only supports following OData query parameters:</span></span>

- <span data-ttu-id="21fd1-120">$expand</span><span class="sxs-lookup"><span data-stu-id="21fd1-120">$expand</span></span>

<span data-ttu-id="21fd1-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="21fd1-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="21fd1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21fd1-122">Request headers</span></span>
|<span data-ttu-id="21fd1-123">Nome</span><span class="sxs-lookup"><span data-stu-id="21fd1-123">Name</span></span>|<span data-ttu-id="21fd1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="21fd1-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="21fd1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="21fd1-125">Authorization</span></span>|<span data-ttu-id="21fd1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21fd1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="21fd1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21fd1-128">Request body</span></span>
<span data-ttu-id="21fd1-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21fd1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21fd1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="21fd1-130">Response</span></span>

<span data-ttu-id="21fd1-131">Se bem-sucedido, este método retorna um código de resposta e um `200 OK` [objeto plannerRoster](../resources/plannerroster.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21fd1-131">If successful, this method returns a `200 OK` response code and a [plannerRoster](../resources/plannerroster.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="21fd1-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="21fd1-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="21fd1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21fd1-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="21fd1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="21fd1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerroster"
}
-->
``` http
GET https://graph.microsoft.com/beta/planner/rosters/6519868f-868f-6519-8f86-19658f861965
```
# <a name="c"></a>[<span data-ttu-id="21fd1-135">C#</span><span class="sxs-lookup"><span data-stu-id="21fd1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerroster-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21fd1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21fd1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerroster-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21fd1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21fd1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerroster-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21fd1-138">Java</span><span class="sxs-lookup"><span data-stu-id="21fd1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerroster-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="21fd1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="21fd1-139">Response</span></span>
<span data-ttu-id="21fd1-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="21fd1-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerRoster"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.plannerRoster",
    "id": "6519868f-868f-6519-8f86-19658f861965"
  }
}
```

