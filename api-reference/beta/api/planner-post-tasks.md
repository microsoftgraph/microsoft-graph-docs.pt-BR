---
title: Criar plannerTask
description: Use essa API para criar um novo **plannerTask**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: f23e2b82857de803add42415a2a91ed99e6725c0
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473805"
---
# <a name="create-plannertask"></a><span data-ttu-id="b5bee-103">Criar plannerTask</span><span class="sxs-lookup"><span data-stu-id="b5bee-103">Create plannerTask</span></span>

<span data-ttu-id="b5bee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5bee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5bee-105">Use essa API para criar um novo **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="b5bee-105">Use this API to create a new **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="b5bee-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5bee-106">Permissions</span></span>
<span data-ttu-id="b5bee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5bee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5bee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5bee-109">Permission type</span></span>      | <span data-ttu-id="b5bee-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5bee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5bee-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5bee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b5bee-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5bee-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5bee-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5bee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5bee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5bee-114">Not supported.</span></span>    |
|<span data-ttu-id="b5bee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5bee-115">Application</span></span> | <span data-ttu-id="b5bee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5bee-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5bee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5bee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/tasks
```
## <a name="request-headers"></a><span data-ttu-id="b5bee-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5bee-118">Request headers</span></span>
| <span data-ttu-id="b5bee-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b5bee-119">Name</span></span>       | <span data-ttu-id="b5bee-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5bee-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b5bee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5bee-121">Authorization</span></span>  | <span data-ttu-id="b5bee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5bee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5bee-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5bee-124">Request body</span></span>
<span data-ttu-id="b5bee-p103">No corpo da solicitação, forneça uma representação JSON do objeto [plannerTask](../resources/plannertask.md). A propriedade planId do **plannerTask** deve ser definida como a id de um objeto [plannerPlan](../resources/plannerplan.md) existente.</span><span class="sxs-lookup"><span data-stu-id="b5bee-p103">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object. The **plannerTask** planId property must be set to an existing [plannerPlan](../resources/plannerplan.md) object's id.</span></span>

## <a name="response"></a><span data-ttu-id="b5bee-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5bee-127">Response</span></span>

<span data-ttu-id="b5bee-128">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [plannerTask](../resources/plannertask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5bee-128">If successful, this method returns `201 Created` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="b5bee-p104">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="b5bee-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="b5bee-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5bee-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5bee-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5bee-133">Request</span></span>
<span data-ttu-id="b5bee-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5bee-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5bee-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5bee-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannertask_from_planner"
}-->
```http
POST https://graph.microsoft.com/beta/planner/tasks
Content-type: application/json
Content-length: 285

{
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "title": "Update client list",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "orderHint": " !"
    }
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="b5bee-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5bee-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannertask-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b5bee-137">C#</span><span class="sxs-lookup"><span data-stu-id="b5bee-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannertask-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b5bee-138">No corpo da solicitação, forneça uma representação JSON do objeto [plannerTask](../resources/plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="b5bee-138">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b5bee-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5bee-139">Response</span></span>
<span data-ttu-id="b5bee-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5bee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 677

{
  "createdBy": {
    "user": {
      "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
    }
  },
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "title": "Update client list",
  "orderHint": "85752723360752+",
  "createdDateTime": "2015-03-25T18:36:49.2407981Z",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:36:49.2407981Z",
      "orderHint": "RWk1"
    }
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


