---
title: Criar plannerPlan
description: Use essa API para criar um novo **plannerPlan**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 37c5ffaec0ff2acf86fc8d5da27868aed8e7707c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036056"
---
# <a name="create-plannerplan"></a><span data-ttu-id="d6eb4-103">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d6eb4-103">Create plannerPlan</span></span>

<span data-ttu-id="d6eb4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6eb4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6eb4-105">Use essa API para criar um novo **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="d6eb4-105">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6eb4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6eb4-106">Permissions</span></span>

<span data-ttu-id="d6eb4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6eb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d6eb4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6eb4-109">Permission type</span></span>                        | <span data-ttu-id="d6eb4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6eb4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d6eb4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6eb4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6eb4-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6eb4-112">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="d6eb4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6eb4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6eb4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6eb4-114">Not supported.</span></span>                              |
| <span data-ttu-id="d6eb4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6eb4-115">Application</span></span>                            | <span data-ttu-id="d6eb4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6eb4-116">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="d6eb4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6eb4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="d6eb4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6eb4-118">Request headers</span></span>

| <span data-ttu-id="d6eb4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d6eb4-119">Name</span></span>          | <span data-ttu-id="d6eb4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6eb4-120">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d6eb4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6eb4-121">Authorization</span></span> | <span data-ttu-id="d6eb4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6eb4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6eb4-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6eb4-124">Request body</span></span>

<span data-ttu-id="d6eb4-p103">No corpo da solicitação, forneça uma representação JSON do objeto [plannerPlan](../resources/plannerplan.md). A propriedade owner do **plannerPlan** deve ser definida com uma identificação de um objeto [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="d6eb4-p103">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

><span data-ttu-id="d6eb4-127">**Observação**: o usuário que está criando o plano deve ser um membro do grupo que será proprietário do plano.</span><span class="sxs-lookup"><span data-stu-id="d6eb4-127">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="d6eb4-128">Ao criar um novo grupo usando [Criar grupo](../api/group-post-groups.md), você não é adicionado ao grupo como membro.</span><span class="sxs-lookup"><span data-stu-id="d6eb4-128">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="d6eb4-129">Depois que o grupo for criado, adicione a si mesmo como membro usando [membros de postagem do grupo](../api/group-post-members.md).</span><span class="sxs-lookup"><span data-stu-id="d6eb4-129">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>

## <a name="response"></a><span data-ttu-id="d6eb4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6eb4-130">Response</span></span>

<span data-ttu-id="d6eb4-131">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6eb4-131">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="d6eb4-p105">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d6eb4-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d6eb4-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6eb4-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6eb4-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6eb4-136">Request</span></span>

<span data-ttu-id="d6eb4-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6eb4-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d6eb4-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6eb4-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
``` http
POST https://graph.microsoft.com/beta/planner/plans
Content-type: application/json
Content-length: 381

{
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d6eb4-139">C#</span><span class="sxs-lookup"><span data-stu-id="d6eb4-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerplan-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6eb4-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6eb4-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerplan-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6eb4-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6eb4-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerplan-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="d6eb4-142">No corpo da solicitação, forneça uma representação JSON do objeto [plannerPlan](../resources/plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="d6eb4-142">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="d6eb4-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6eb4-143">Response</span></span>

<span data-ttu-id="d6eb4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6eb4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
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


