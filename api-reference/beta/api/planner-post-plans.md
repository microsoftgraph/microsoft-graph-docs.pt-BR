---
title: Criar plannerPlan
description: Use essa API para criar um novo **plannerPlan**.
ms.openlocfilehash: 685b05cc271aaebfdb198eace416883c52ad28a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038685"
---
# <a name="create-plannerplan"></a><span data-ttu-id="fe631-103">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="fe631-103">Create plannerPlan</span></span>

> <span data-ttu-id="fe631-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fe631-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe631-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fe631-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe631-106">Use essa API para criar um novo **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="fe631-106">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe631-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe631-107">Permissions</span></span>

<span data-ttu-id="fe631-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe631-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fe631-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe631-110">Permission type</span></span>                        | <span data-ttu-id="fe631-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe631-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="fe631-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe631-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe631-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe631-113">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="fe631-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe631-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe631-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe631-115">Not supported.</span></span>                              |
| <span data-ttu-id="fe631-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe631-116">Application</span></span>                            | <span data-ttu-id="fe631-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe631-117">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="fe631-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe631-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="fe631-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe631-119">Request headers</span></span>

| <span data-ttu-id="fe631-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fe631-120">Name</span></span>          | <span data-ttu-id="fe631-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe631-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fe631-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe631-122">Authorization</span></span> | <span data-ttu-id="fe631-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe631-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe631-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe631-125">Request body</span></span>

<span data-ttu-id="fe631-p104">No corpo da solicitação, forneça uma representação JSON do objeto [plannerPlan](../resources/plannerplan.md). A propriedade owner do **plannerPlan** deve ser definida com uma identificação de um objeto [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="fe631-p104">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

><span data-ttu-id="fe631-128">**Observação:** O usuário que está criando o plano deve ser um membro do grupo que será o proprietário do plano.</span><span class="sxs-lookup"><span data-stu-id="fe631-128">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="fe631-129">Quando você cria um novo grupo usando [Criar grupo](../api/group-post-groups.md), você não é adicionados ao grupo como um membro.</span><span class="sxs-lookup"><span data-stu-id="fe631-129">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="fe631-130">Depois que o grupo é criado, adicione si mesmo como membro usando o [grupo postar membros](../api/group-post-members.md).</span><span class="sxs-lookup"><span data-stu-id="fe631-130">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>

## <a name="response"></a><span data-ttu-id="fe631-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe631-131">Response</span></span>

<span data-ttu-id="fe631-132">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe631-132">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="fe631-p106">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="fe631-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="fe631-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe631-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe631-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe631-137">Request</span></span>

<span data-ttu-id="fe631-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe631-138">Here is an example of the request.</span></span>
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

<span data-ttu-id="fe631-139">No corpo da solicitação, forneça uma representação JSON do objeto [plannerPlan](../resources/plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="fe631-139">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="fe631-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe631-140">Response</span></span>

<span data-ttu-id="fe631-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe631-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->