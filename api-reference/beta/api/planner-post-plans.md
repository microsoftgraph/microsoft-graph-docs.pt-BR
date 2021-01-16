---
title: Criar plannerPlan
description: Use essa API para criar um novo **plannerPlan**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: f56bab29e538afd8841ddd86a57b6a5456b969d8
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883197"
---
# <a name="create-plannerplan"></a><span data-ttu-id="dc1db-103">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="dc1db-103">Create plannerPlan</span></span>

<span data-ttu-id="dc1db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc1db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc1db-105">Crie um novo **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="dc1db-105">Create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc1db-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="dc1db-106">Permissions</span></span>

<span data-ttu-id="dc1db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc1db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dc1db-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc1db-109">Permission type</span></span>                        | <span data-ttu-id="dc1db-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc1db-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="dc1db-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc1db-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dc1db-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc1db-112">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="dc1db-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc1db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc1db-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc1db-114">Not supported.</span></span>                              |
| <span data-ttu-id="dc1db-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc1db-115">Application</span></span>                            | <span data-ttu-id="dc1db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc1db-116">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="dc1db-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc1db-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="dc1db-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc1db-118">Request headers</span></span>

| <span data-ttu-id="dc1db-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dc1db-119">Name</span></span>          | <span data-ttu-id="dc1db-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc1db-120">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="dc1db-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc1db-121">Authorization</span></span> | <span data-ttu-id="dc1db-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc1db-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dc1db-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="dc1db-124">Content-type</span></span> | <span data-ttu-id="dc1db-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc1db-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc1db-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc1db-127">Request body</span></span>

<span data-ttu-id="dc1db-128">No corpo da solicitação, forneça uma representação JSON do objeto [plannerPlan](../resources/plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="dc1db-128">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>
<span data-ttu-id="dc1db-129">A propriedade do contêiner **plannerPlan** deve ser definida.</span><span class="sxs-lookup"><span data-stu-id="dc1db-129">The **plannerPlan** container property must be set.</span></span>

><span data-ttu-id="dc1db-130">**Observação:** Se o contêiner for um grupo do Microsoft 365, o usuário que está criando o plano deverá ser um membro do grupo que conterá o plano.</span><span class="sxs-lookup"><span data-stu-id="dc1db-130">**Note:** If the container is a Microsoft 365 group, the user who is creating the plan must be a member of the group that will contain the plan.</span></span> <span data-ttu-id="dc1db-131">Ao criar um novo grupo usando [Criar grupo](../api/group-post-groups.md), você não é adicionado ao grupo como membro.</span><span class="sxs-lookup"><span data-stu-id="dc1db-131">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="dc1db-132">Depois que o grupo for criado, adicione a si mesmo como membro usando [membros de postagem do grupo](../api/group-post-members.md).</span><span class="sxs-lookup"><span data-stu-id="dc1db-132">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>

## <a name="response"></a><span data-ttu-id="dc1db-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc1db-133">Response</span></span>

<span data-ttu-id="dc1db-134">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc1db-134">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="dc1db-p106">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="dc1db-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="dc1db-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc1db-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc1db-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc1db-139">Request</span></span>

<span data-ttu-id="dc1db-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc1db-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dc1db-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc1db-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
``` http
POST https://graph.microsoft.com/beta/planner/plans
Content-type: application/json
Content-length: 140

{
  "container": {
    "url": "https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874"
  },
  "title": "title-value"
}
```
# <a name="c"></a>[<span data-ttu-id="dc1db-142">C#</span><span class="sxs-lookup"><span data-stu-id="dc1db-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerplan-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc1db-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc1db-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerplan-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc1db-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc1db-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerplan-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dc1db-145">Java</span><span class="sxs-lookup"><span data-stu-id="dc1db-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerplan-from-planner-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dc1db-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc1db-146">Response</span></span>

<span data-ttu-id="dc1db-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc1db-147">Here is an example of the response.</span></span> 

><span data-ttu-id="dc1db-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dc1db-148">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
``` http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 544

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "b108ebf3-4e22-b93d-5234-dae5874656d7"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "container": {
    "@odata.type": "microsoft.graph.plannerPlanContainer",
    "url": "https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874",
    "containerId": "ebf3b108-5234-4e22-b93d-656d7dae5874",
    "type": "group"
  },
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


