---
title: Criar plannerPlan
description: Use essa API para criar um novo **plannerPlan**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 83bd7f04e6f4a5064e0deabf253bb99788610744
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881256"
---
# <a name="create-plannerplan"></a><span data-ttu-id="4f206-103">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="4f206-103">Create plannerPlan</span></span>

<span data-ttu-id="4f206-104">Use essa API para criar um novo **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="4f206-104">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f206-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f206-105">Permissions</span></span>

<span data-ttu-id="4f206-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f206-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f206-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f206-108">Permission type</span></span>                        | <span data-ttu-id="4f206-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f206-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="4f206-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f206-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f206-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f206-111">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="4f206-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f206-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f206-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f206-113">Not supported.</span></span>                              |
| <span data-ttu-id="4f206-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f206-114">Application</span></span>                            | <span data-ttu-id="4f206-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f206-115">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="4f206-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f206-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="4f206-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f206-117">Request headers</span></span>

| <span data-ttu-id="4f206-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4f206-118">Name</span></span>          | <span data-ttu-id="4f206-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f206-119">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4f206-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f206-120">Authorization</span></span> | <span data-ttu-id="4f206-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f206-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f206-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f206-123">Request body</span></span>

<span data-ttu-id="4f206-p103">No corpo da solicitação, forneça uma representação JSON do objeto [plannerPlan](../resources/plannerplan.md). A propriedade owner do **plannerPlan** deve ser definida com uma identificação de um objeto [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="4f206-p103">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

><span data-ttu-id="4f206-126">**Observação**: o usuário que está criando o plano deve ser um membro do grupo que será proprietário do plano.</span><span class="sxs-lookup"><span data-stu-id="4f206-126">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="4f206-127">Ao criar um novo grupo usando [Criar grupo](../api/group-post-groups.md), você não é adicionado ao grupo como membro.</span><span class="sxs-lookup"><span data-stu-id="4f206-127">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="4f206-128">Depois que o grupo for criado, adicione a si mesmo como membro usando [membros de postagem do grupo](../api/group-post-members.md).</span><span class="sxs-lookup"><span data-stu-id="4f206-128">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>


## <a name="response"></a><span data-ttu-id="4f206-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f206-129">Response</span></span>

<span data-ttu-id="4f206-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f206-130">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="4f206-p105">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="4f206-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4f206-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f206-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f206-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f206-135">Request</span></span>

<span data-ttu-id="4f206-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f206-136">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4f206-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f206-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
``` http
POST https://graph.microsoft.com/v1.0/planner/plans
Content-type: application/json
Content-length: 381

{
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4f206-138">C#</span><span class="sxs-lookup"><span data-stu-id="4f206-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerplan-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f206-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="4f206-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerplan-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4f206-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4f206-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerplan-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4f206-141">Java</span><span class="sxs-lookup"><span data-stu-id="4f206-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerplan-from-planner-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="4f206-142">No corpo da solicitação, forneça uma representação JSON do objeto [plannerPlan](../resources/plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="4f206-142">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="4f206-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f206-143">Response</span></span>

<span data-ttu-id="4f206-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f206-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
