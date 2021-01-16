---
title: Atualizar plannerPlan
description: Atualizar as propriedades de um **objeto plannerPlan.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 30a0c76d4e2d1a84d897edeadfd7370448ce7b80
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882884"
---
# <a name="update-plannerplan"></a><span data-ttu-id="40520-103">Atualizar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="40520-103">Update plannerPlan</span></span>

<span data-ttu-id="40520-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40520-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40520-105">Atualizar as propriedades de um **objeto plannerPlan.**</span><span class="sxs-lookup"><span data-stu-id="40520-105">Update the properties of a **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="40520-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="40520-106">Permissions</span></span>
<span data-ttu-id="40520-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40520-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40520-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40520-109">Permission type</span></span>      | <span data-ttu-id="40520-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40520-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40520-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40520-111">Delegated (work or school account)</span></span> | <span data-ttu-id="40520-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40520-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="40520-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40520-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40520-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40520-114">Not supported.</span></span>    |
|<span data-ttu-id="40520-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40520-115">Application</span></span> | <span data-ttu-id="40520-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40520-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40520-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40520-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{plan-id}
```

## <a name="request-headers"></a><span data-ttu-id="40520-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40520-118">Request headers</span></span>

| <span data-ttu-id="40520-119">Nome</span><span class="sxs-lookup"><span data-stu-id="40520-119">Name</span></span>       | <span data-ttu-id="40520-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="40520-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="40520-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="40520-121">Authorization</span></span>  | <span data-ttu-id="40520-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40520-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40520-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="40520-124">If-Match</span></span>  | <span data-ttu-id="40520-125">Último valor ETag conhecido para o plannerPlan a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="40520-125">Last known ETag value for the plannerPlan to be updated.</span></span> <span data-ttu-id="40520-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40520-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40520-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40520-127">Request body</span></span>
<span data-ttu-id="40520-128">No corpo da solicitação, fornece os valores dos campos relevantes a atualizar.</span><span class="sxs-lookup"><span data-stu-id="40520-128">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="40520-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="40520-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="40520-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="40520-130">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="40520-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="40520-131">Response</span></span>

<span data-ttu-id="40520-132">Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto [plannerPlan](../resources/plannerplan.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40520-132">If successful, this method returns a `200 OK` response code and an updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="40520-p105">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="40520-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="40520-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40520-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40520-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40520-137">Request</span></span>
<span data-ttu-id="40520-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40520-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="40520-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="40520-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/plans/{id}
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
# <a name="c"></a>[<span data-ttu-id="40520-140">C#</span><span class="sxs-lookup"><span data-stu-id="40520-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40520-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40520-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40520-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40520-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40520-143">Java</span><span class="sxs-lookup"><span data-stu-id="40520-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerplan-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="40520-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="40520-144">Response</span></span>
<span data-ttu-id="40520-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40520-145">Here is an example of the response.</span></span> 

><span data-ttu-id="40520-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40520-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
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
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


