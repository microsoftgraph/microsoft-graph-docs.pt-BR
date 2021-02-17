---
title: Criar plannerRoster
description: Crie um novo objeto plannerRoster.
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 153a88951943ce1a66d73ee26be289eaae7631f0
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271999"
---
# <a name="create-plannerroster"></a><span data-ttu-id="7a172-103">Criar plannerRoster</span><span class="sxs-lookup"><span data-stu-id="7a172-103">Create plannerRoster</span></span>
<span data-ttu-id="7a172-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a172-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a172-105">Crie um novo [objeto plannerRoster.](../resources/plannerroster.md)</span><span class="sxs-lookup"><span data-stu-id="7a172-105">Create a new [plannerRoster](../resources/plannerroster.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a172-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7a172-106">Permissions</span></span>
<span data-ttu-id="7a172-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a172-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a172-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a172-109">Permission type</span></span>|<span data-ttu-id="7a172-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a172-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a172-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a172-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7a172-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a172-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="7a172-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a172-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a172-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a172-114">Not supported.</span></span>|
|<span data-ttu-id="7a172-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a172-115">Application</span></span>|<span data-ttu-id="7a172-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a172-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a172-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a172-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /planner/rosters
```

## <a name="request-headers"></a><span data-ttu-id="7a172-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a172-118">Request headers</span></span>
|<span data-ttu-id="7a172-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7a172-119">Name</span></span>|<span data-ttu-id="7a172-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a172-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7a172-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a172-121">Authorization</span></span>|<span data-ttu-id="7a172-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a172-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7a172-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a172-124">Content-Type</span></span>|<span data-ttu-id="7a172-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a172-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a172-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a172-127">Request body</span></span>
<span data-ttu-id="7a172-128">No corpo da solicitação, fornece uma representação JSON do [objeto plannerRoster.](../resources/plannerroster.md)</span><span class="sxs-lookup"><span data-stu-id="7a172-128">In the request body, supply a JSON representation of the [plannerRoster](../resources/plannerroster.md) object.</span></span>

<span data-ttu-id="7a172-129">Não há propriedades writable no [plannerRoster](../resources/plannerroster.md).</span><span class="sxs-lookup"><span data-stu-id="7a172-129">There are no writable properties on [plannerRoster](../resources/plannerroster.md).</span></span>

## <a name="response"></a><span data-ttu-id="7a172-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a172-130">Response</span></span>

<span data-ttu-id="7a172-131">Se bem-sucedido, este método retorna um código de resposta e um `201 Created` [objeto plannerRoster](../resources/plannerroster.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a172-131">If successful, this method returns a `201 Created` response code and a [plannerRoster](../resources/plannerroster.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7a172-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7a172-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7a172-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a172-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7a172-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a172-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerroster_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/planner/rosters
Content-Type: application/json
Content-length: 55

{
  "@odata.type": "#microsoft.graph.plannerRoster"
}
```
# <a name="c"></a>[<span data-ttu-id="7a172-135">C#</span><span class="sxs-lookup"><span data-stu-id="7a172-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerroster-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a172-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a172-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerroster-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a172-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a172-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerroster-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a172-138">Java</span><span class="sxs-lookup"><span data-stu-id="7a172-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerroster-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7a172-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a172-139">Response</span></span>
<span data-ttu-id="7a172-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7a172-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerRoster"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.plannerRoster",
  "id": "6519868f-868f-6519-8f86-19658f861965"
}
```

