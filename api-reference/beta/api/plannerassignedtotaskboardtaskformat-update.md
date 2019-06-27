---
title: Atualizar plannerAssignedToTaskBoardTaskFormat
description: Atualize as propriedades do objeto **plannerAssignedToTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 93db40e26af2f07222870d2bf2a8151e515b23e4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268345"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="d9cee-103">Atualizar plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d9cee-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9cee-104">Atualize as propriedades do objeto **plannerAssignedToTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="d9cee-104">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d9cee-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9cee-105">Permissions</span></span>
<span data-ttu-id="d9cee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9cee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9cee-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9cee-108">Permission type</span></span>      | <span data-ttu-id="d9cee-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9cee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9cee-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9cee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d9cee-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9cee-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d9cee-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9cee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9cee-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9cee-113">Not supported.</span></span>    |
|<span data-ttu-id="d9cee-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9cee-114">Application</span></span> | <span data-ttu-id="d9cee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9cee-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9cee-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9cee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="d9cee-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="d9cee-117">Optional request headers</span></span>
| <span data-ttu-id="d9cee-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d9cee-118">Name</span></span>       | <span data-ttu-id="d9cee-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9cee-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d9cee-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9cee-120">Authorization</span></span>  | <span data-ttu-id="d9cee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9cee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d9cee-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="d9cee-123">If-Match</span></span>  | <span data-ttu-id="d9cee-124">O último valor de ETag conhecido para **plannerAssignedToTaskBoardTaskFormat** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="d9cee-124">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated.</span></span> <span data-ttu-id="d9cee-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9cee-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9cee-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9cee-126">Request body</span></span>
<span data-ttu-id="d9cee-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d9cee-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d9cee-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9cee-130">Property</span></span>     | <span data-ttu-id="d9cee-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9cee-131">Type</span></span>   |<span data-ttu-id="d9cee-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9cee-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9cee-133">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="d9cee-133">orderHintsByAssignee</span></span>|[<span data-ttu-id="d9cee-134">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="d9cee-134">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="d9cee-135">Dicionário de dicas usado para ordenar tarefas na exibição AssignedTo do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d9cee-135">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board.</span></span> <span data-ttu-id="d9cee-136">A chave de cada entrada é um dos usuários para os quais a tarefa é atribuída e o valor é a dica ORDER.</span><span class="sxs-lookup"><span data-stu-id="d9cee-136">The key of each entry is one of the users the task is assigned to and the value is the order hint.</span></span> <span data-ttu-id="d9cee-137">O formato de cada valor é definido em [using Order Hints in Planner (.. /resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="d9cee-137">The format of each value is defined in [Using order hints in Planner(../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="d9cee-138">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="d9cee-138">unassignedOrderHint</span></span>|<span data-ttu-id="d9cee-139">String</span><span class="sxs-lookup"><span data-stu-id="d9cee-139">String</span></span>|<span data-ttu-id="d9cee-140">O valor de dica usado para ordenar a tarefa na exibição AssignedTo do quadro de tarefas quando a tarefa não é atribuída a qualquer pessoa ou quando o dicionário do orderHintsByAssignee não fornece uma dica de pedido para o usuário ao qual a tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="d9cee-140">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to.</span></span> <span data-ttu-id="d9cee-141">O formato é definido em [usando dicas de ordenação no Planner](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="d9cee-141">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="d9cee-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9cee-142">Response</span></span>

<span data-ttu-id="d9cee-143">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9cee-143">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="d9cee-p107">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d9cee-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d9cee-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9cee-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9cee-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9cee-148">Request</span></span>
<span data-ttu-id="d9cee-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9cee-149">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="d9cee-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9cee-150">Response</span></span>
<span data-ttu-id="d9cee-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9cee-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d9cee-154">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d9cee-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d9cee-155">C#</span><span class="sxs-lookup"><span data-stu-id="d9cee-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_plannerassignedtotaskboardtaskformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d9cee-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="d9cee-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_plannerassignedtotaskboardtaskformat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d9cee-157">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d9cee-157">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_plannerassignedtotaskboardtaskformat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/plannerassignedtotaskboardtaskformat-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/plannerassignedtotaskboardtaskformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/plannerassignedtotaskboardtaskformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
