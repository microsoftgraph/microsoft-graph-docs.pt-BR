---
title: Atualizar plannerAssignedToTaskBoardTaskFormat
description: Atualize as propriedades **do objeto plannerAssignedToTaskBoardTaskFormat.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: e05a358c49443dea5a44185b5dc38c629a3aedce
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473910"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="cdfbc-103">Atualizar plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="cdfbc-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="cdfbc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdfbc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdfbc-105">Atualize as propriedades **do objeto plannerAssignedToTaskBoardTaskFormat.**</span><span class="sxs-lookup"><span data-stu-id="cdfbc-105">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cdfbc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cdfbc-106">Permissions</span></span>
<span data-ttu-id="cdfbc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdfbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdfbc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdfbc-109">Permission type</span></span>      | <span data-ttu-id="cdfbc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cdfbc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdfbc-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdfbc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cdfbc-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdfbc-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cdfbc-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdfbc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdfbc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdfbc-114">Not supported.</span></span>    |
|<span data-ttu-id="cdfbc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdfbc-115">Application</span></span> | <span data-ttu-id="cdfbc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdfbc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdfbc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdfbc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="cdfbc-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="cdfbc-118">Optional request headers</span></span>
| <span data-ttu-id="cdfbc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cdfbc-119">Name</span></span>       | <span data-ttu-id="cdfbc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdfbc-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cdfbc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdfbc-121">Authorization</span></span>  | <span data-ttu-id="cdfbc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdfbc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cdfbc-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="cdfbc-124">If-Match</span></span>  | <span data-ttu-id="cdfbc-125">Último valor de ETag conhecido **para plannerAssignedToTaskBoardTaskFormat** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="cdfbc-125">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated.</span></span> <span data-ttu-id="cdfbc-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdfbc-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdfbc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdfbc-127">Request body</span></span>
<span data-ttu-id="cdfbc-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="cdfbc-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cdfbc-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cdfbc-131">Property</span></span>     | <span data-ttu-id="cdfbc-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdfbc-132">Type</span></span>   |<span data-ttu-id="cdfbc-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdfbc-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cdfbc-134">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="cdfbc-134">orderHintsByAssignee</span></span>|[<span data-ttu-id="cdfbc-135">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="cdfbc-135">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="cdfbc-136">Dicionário de dicas usadas para ordenar tarefas no modo de exibição AssignedTo do Quadro de Tarefas.</span><span class="sxs-lookup"><span data-stu-id="cdfbc-136">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board.</span></span> <span data-ttu-id="cdfbc-137">A chave de cada entrada é um dos usuários aos qual a tarefa é atribuída e o valor é a dica de pedido.</span><span class="sxs-lookup"><span data-stu-id="cdfbc-137">The key of each entry is one of the users the task is assigned to and the value is the order hint.</span></span> <span data-ttu-id="cdfbc-138">O formato de cada valor é definido em [Usando dicas de ordem no Planner(.). /resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="cdfbc-138">The format of each value is defined in [Using order hints in Planner(../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="cdfbc-139">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="cdfbc-139">unassignedOrderHint</span></span>|<span data-ttu-id="cdfbc-140">String</span><span class="sxs-lookup"><span data-stu-id="cdfbc-140">String</span></span>|<span data-ttu-id="cdfbc-141">Valor de dica usado para ordenar a tarefa no modo de exibição AssignedTo do Quadro de Tarefas quando a tarefa não é atribuída a ninguém ou se o dicionário orderHintsByAssignee não fornecer uma dica de ordem para o usuário ao qual a tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="cdfbc-141">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to.</span></span> <span data-ttu-id="cdfbc-142">O formato é definido em [Usando dicas de ordem no Planner](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="cdfbc-142">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="cdfbc-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdfbc-143">Response</span></span>

<span data-ttu-id="cdfbc-144">Se tiver êxito, este método retornará `204 No Content` resposta e conteúdo vazio.</span><span class="sxs-lookup"><span data-stu-id="cdfbc-144">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="cdfbc-145">Se a solicitação especificar o header com preferência, este método retornará um código de resposta e o `Prefer` `return=representation` objeto `200 OK` [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdfbc-145">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="cdfbc-p108">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="cdfbc-p108">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="cdfbc-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdfbc-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cdfbc-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdfbc-150">Request</span></span>
<span data-ttu-id="cdfbc-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdfbc-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cdfbc-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdfbc-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat
Content-type: application/json
Content-length: 96
Prefer: return=representation
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHintsByAssignee": {
    "aaa27244-1db4-476a-a5cb-004607466324": "8566473P 957764Jk!"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="cdfbc-153">C#</span><span class="sxs-lookup"><span data-stu-id="cdfbc-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerassignedtotaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdfbc-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdfbc-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerassignedtotaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdfbc-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdfbc-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerassignedtotaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cdfbc-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdfbc-156">Response</span></span>
<span data-ttu-id="cdfbc-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cdfbc-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "unassignedOrderHint": "RWk1",
  "orderHintsByAssignee": {
    "6463a5ce-2119-4198-9f2a-628761df4a62":"85752723360752+",
    "aaa27244-1db4-476a-a5cb-004607466324":"90057581;"
  },
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerassignedtotaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


