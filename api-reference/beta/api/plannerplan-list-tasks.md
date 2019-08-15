---
title: Listar tarefas
description: Recupere uma lista de objetos **plannerTask** associados a um objeto plannerPlan.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: c50d658756b677d426ce70b68d8b10ebd63b5ac8
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413262"
---
# <a name="list-tasks"></a><span data-ttu-id="5ccb2-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="5ccb2-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ccb2-104">Recupere uma lista de objetos [plannerTask](../resources/plannertask.md) associados a um objeto [plannerPlan](../resources/plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="5ccb2-104">Retrieve a list of [plannerTask](../resources/plannertask.md) objects associated with a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5ccb2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ccb2-105">Permissions</span></span>
<span data-ttu-id="5ccb2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ccb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ccb2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ccb2-108">Permission type</span></span>      | <span data-ttu-id="5ccb2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ccb2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ccb2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ccb2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5ccb2-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ccb2-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5ccb2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ccb2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ccb2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ccb2-113">Not supported.</span></span>    |
|<span data-ttu-id="5ccb2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ccb2-114">Application</span></span> | <span data-ttu-id="5ccb2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ccb2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ccb2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ccb2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{plan-id}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="5ccb2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ccb2-117">Request headers</span></span>
| <span data-ttu-id="5ccb2-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5ccb2-118">Name</span></span>      |<span data-ttu-id="5ccb2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ccb2-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5ccb2-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ccb2-120">Authorization</span></span>  | <span data-ttu-id="5ccb2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ccb2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ccb2-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ccb2-123">Request body</span></span>
<span data-ttu-id="5ccb2-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ccb2-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ccb2-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ccb2-125">Response</span></span>

<span data-ttu-id="5ccb2-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [plannerTask](../resources/plannertask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ccb2-126">If successful, this method returns a `200 OK` response code and a collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="5ccb2-127">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="5ccb2-127">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="5ccb2-128">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="5ccb2-128">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="5ccb2-129">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="5ccb2-129">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="5ccb2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ccb2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ccb2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ccb2-131">Request</span></span>
<span data-ttu-id="5ccb2-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ccb2-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5ccb2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ccb2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/tasks
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5ccb2-134">C#</span><span class="sxs-lookup"><span data-stu-id="5ccb2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5ccb2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ccb2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5ccb2-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5ccb2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5ccb2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ccb2-137">Response</span></span>
<span data-ttu-id="5ccb2-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ccb2-138">Here is an example of the response.</span></span> 

><span data-ttu-id="5ccb2-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ccb2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 833

{
  "value": [
    {
      "createdBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
      "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
      "title": "title-value",
      "orderHint": "9223370609546166567W",
      "assigneePriority": "90057581\"",
      "createdDateTime": "2015-03-25T18:36:49.2407981Z",
      "assignments": {
        "fbab97d0-4932-4511-b675-204639209557": {
          "@odata.type": "#microsoft.graph.plannerAssignment",
          "assignedBy": {
            "user": {
              "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
            }
          },
          "assignedDateTime": "2015-03-25T18:38:21.956Z",
          "orderHint": "RWk1"
         }
      },
      "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
