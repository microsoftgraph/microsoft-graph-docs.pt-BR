---
title: Atualizar plannerAssignedToTaskBoardTaskFormat
description: Atualize as propriedades do objeto **plannerAssignedToTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 885eb25e57cb31ff3e5c0f291b9fbcf529ea06ce
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342303"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="131c3-103">Atualizar plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="131c3-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="131c3-104">Atualize as propriedades do objeto **plannerAssignedToTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="131c3-104">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="131c3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="131c3-105">Permissions</span></span>
<span data-ttu-id="131c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="131c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="131c3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="131c3-108">Permission type</span></span>      | <span data-ttu-id="131c3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="131c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="131c3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="131c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="131c3-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="131c3-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="131c3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="131c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="131c3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="131c3-113">Not supported.</span></span>    |
|<span data-ttu-id="131c3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="131c3-114">Application</span></span> | <span data-ttu-id="131c3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="131c3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="131c3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="131c3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="131c3-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="131c3-117">Optional request headers</span></span>
| <span data-ttu-id="131c3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="131c3-118">Name</span></span>       | <span data-ttu-id="131c3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="131c3-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="131c3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="131c3-120">Authorization</span></span>  | <span data-ttu-id="131c3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="131c3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="131c3-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="131c3-123">If-Match</span></span>  | <span data-ttu-id="131c3-124">O último valor de ETag conhecido para **plannerAssignedToTaskBoardTaskFormat** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="131c3-124">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated.</span></span> <span data-ttu-id="131c3-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="131c3-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="131c3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="131c3-126">Request body</span></span>
<span data-ttu-id="131c3-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="131c3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="131c3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="131c3-130">Property</span></span>     | <span data-ttu-id="131c3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="131c3-131">Type</span></span>   |<span data-ttu-id="131c3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="131c3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="131c3-133">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="131c3-133">orderHintsByAssignee</span></span>|[<span data-ttu-id="131c3-134">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="131c3-134">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="131c3-135">Dicionário de dicas usado para ordenar tarefas na exibição AssignedTo do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="131c3-135">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board.</span></span> <span data-ttu-id="131c3-136">A chave de cada entrada é um dos usuários para os quais a tarefa é atribuída e o valor é a dica ORDER.</span><span class="sxs-lookup"><span data-stu-id="131c3-136">The key of each entry is one of the users the task is assigned to and the value is the order hint.</span></span> <span data-ttu-id="131c3-137">O formato de cada valor é definido em [using Order Hints in Planner (.. /resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="131c3-137">The format of each value is defined in [Using order hints in Planner(../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="131c3-138">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="131c3-138">unassignedOrderHint</span></span>|<span data-ttu-id="131c3-139">String</span><span class="sxs-lookup"><span data-stu-id="131c3-139">String</span></span>|<span data-ttu-id="131c3-140">O valor de dica usado para ordenar a tarefa na exibição AssignedTo do quadro de tarefas quando a tarefa não é atribuída a qualquer pessoa ou quando o dicionário do orderHintsByAssignee não fornece uma dica de pedido para o usuário ao qual a tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="131c3-140">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to.</span></span> <span data-ttu-id="131c3-141">O formato é definido em [usando dicas de ordenação no Planner](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="131c3-141">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="131c3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="131c3-142">Response</span></span>

<span data-ttu-id="131c3-143">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="131c3-143">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="131c3-p107">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="131c3-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="131c3-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="131c3-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="131c3-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="131c3-148">Request</span></span>
<span data-ttu-id="131c3-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="131c3-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="131c3-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="131c3-150">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="131c3-151">C#</span><span class="sxs-lookup"><span data-stu-id="131c3-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerassignedtotaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="131c3-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="131c3-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerassignedtotaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="131c3-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="131c3-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerassignedtotaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="131c3-154">Java</span><span class="sxs-lookup"><span data-stu-id="131c3-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerassignedtotaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="131c3-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="131c3-155">Response</span></span>
<span data-ttu-id="131c3-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="131c3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
