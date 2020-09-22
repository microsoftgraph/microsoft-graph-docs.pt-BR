---
title: Atualizar plannerAssignedToTaskBoardTaskFormat
description: Atualize as propriedades do objeto **plannerAssignedToTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 048936a5d1a4c2f311a8d7bea483e01486ed2afb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081913"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="72431-103">Atualizar plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="72431-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="72431-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72431-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72431-105">Atualize as propriedades do objeto **plannerAssignedToTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="72431-105">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="72431-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="72431-106">Permissions</span></span>
<span data-ttu-id="72431-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72431-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72431-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72431-109">Permission type</span></span>      | <span data-ttu-id="72431-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72431-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72431-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72431-111">Delegated (work or school account)</span></span> | <span data-ttu-id="72431-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72431-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="72431-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72431-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72431-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72431-114">Not supported.</span></span>    |
|<span data-ttu-id="72431-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72431-115">Application</span></span> | <span data-ttu-id="72431-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72431-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72431-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72431-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="72431-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="72431-118">Optional request headers</span></span>
| <span data-ttu-id="72431-119">Nome</span><span class="sxs-lookup"><span data-stu-id="72431-119">Name</span></span>       | <span data-ttu-id="72431-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="72431-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="72431-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="72431-121">Authorization</span></span>  | <span data-ttu-id="72431-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72431-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="72431-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="72431-124">If-Match</span></span>  | <span data-ttu-id="72431-125">O último valor de ETag conhecido para **plannerAssignedToTaskBoardTaskFormat** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="72431-125">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated.</span></span> <span data-ttu-id="72431-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72431-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="72431-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72431-127">Request body</span></span>
<span data-ttu-id="72431-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="72431-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="72431-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72431-131">Property</span></span>     | <span data-ttu-id="72431-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="72431-132">Type</span></span>   |<span data-ttu-id="72431-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="72431-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72431-134">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="72431-134">orderHintsByAssignee</span></span>|[<span data-ttu-id="72431-135">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="72431-135">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="72431-136">Dicionário de dicas usado para ordenar tarefas na exibição AssignedTo do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="72431-136">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board.</span></span> <span data-ttu-id="72431-137">A chave de cada entrada é um dos usuários para os quais a tarefa é atribuída e o valor é a dica ORDER.</span><span class="sxs-lookup"><span data-stu-id="72431-137">The key of each entry is one of the users the task is assigned to and the value is the order hint.</span></span> <span data-ttu-id="72431-138">O formato de cada valor é definido em [using Order Hints in Planner (.. /Resources/planner_order_hint_format. MD).</span><span class="sxs-lookup"><span data-stu-id="72431-138">The format of each value is defined in [Using order hints in Planner(../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="72431-139">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="72431-139">unassignedOrderHint</span></span>|<span data-ttu-id="72431-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72431-140">String</span></span>|<span data-ttu-id="72431-141">O valor de dica usado para ordenar a tarefa na exibição AssignedTo do quadro de tarefas quando a tarefa não é atribuída a qualquer pessoa ou quando o dicionário do orderHintsByAssignee não fornece uma dica de pedido para o usuário ao qual a tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="72431-141">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to.</span></span> <span data-ttu-id="72431-142">O formato é definido em [usando dicas de ordenação no Planner](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="72431-142">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="72431-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="72431-143">Response</span></span>

<span data-ttu-id="72431-144">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72431-144">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="72431-p107">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="72431-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="72431-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72431-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72431-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72431-149">Request</span></span>
<span data-ttu-id="72431-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72431-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72431-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="72431-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat
Content-type: application/json
Content-length: 96
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHintsByAssignee": {
    "aaa27244-1db4-476a-a5cb-004607466324": "8566473P 957764Jk!"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="72431-152">C#</span><span class="sxs-lookup"><span data-stu-id="72431-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerassignedtotaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72431-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72431-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerassignedtotaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72431-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72431-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerassignedtotaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="72431-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="72431-155">Response</span></span>
<span data-ttu-id="72431-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72431-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


