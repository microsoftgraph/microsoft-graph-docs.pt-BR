---
title: Atualizar plannerAssignedToTaskBoardTaskFormat
description: Atualize as propriedades do objeto **plannerAssignedToTaskBoardTaskFormat**.
localization_priority: Normal
ms.openlocfilehash: 2586e0d413ce6debcc90b720c2ec45773518507e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856801"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="04a25-103">Atualizar plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="04a25-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

> <span data-ttu-id="04a25-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="04a25-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04a25-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="04a25-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="04a25-106">Atualize as propriedades do objeto **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="04a25-106">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="04a25-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="04a25-107">Permissions</span></span>
<span data-ttu-id="04a25-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04a25-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04a25-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04a25-110">Permission type</span></span>      | <span data-ttu-id="04a25-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04a25-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04a25-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04a25-112">Delegated (work or school account)</span></span> | <span data-ttu-id="04a25-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04a25-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="04a25-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04a25-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04a25-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04a25-115">Not supported.</span></span>    |
|<span data-ttu-id="04a25-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04a25-116">Application</span></span> | <span data-ttu-id="04a25-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04a25-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04a25-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04a25-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="04a25-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="04a25-119">Optional request headers</span></span>
| <span data-ttu-id="04a25-120">Nome</span><span class="sxs-lookup"><span data-stu-id="04a25-120">Name</span></span>       | <span data-ttu-id="04a25-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="04a25-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="04a25-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="04a25-122">Authorization</span></span>  | <span data-ttu-id="04a25-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04a25-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="04a25-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="04a25-125">If-Match</span></span>  | <span data-ttu-id="04a25-p104">Último valor ETag conhecido do objeto **plannerAssignedToTaskBoardTaskFormat** a ser atualizado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04a25-p104">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04a25-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04a25-128">Request body</span></span>
<span data-ttu-id="04a25-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="04a25-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="04a25-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04a25-132">Property</span></span>     | <span data-ttu-id="04a25-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="04a25-133">Type</span></span>   |<span data-ttu-id="04a25-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="04a25-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04a25-135">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="04a25-135">orderHintsByAssignee</span></span>|[<span data-ttu-id="04a25-136">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="04a25-136">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="04a25-137">Dicionário de dicas usado para tarefas de ordem na exibição AssignedTo da placa de tarefa.</span><span class="sxs-lookup"><span data-stu-id="04a25-137">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board.</span></span> <span data-ttu-id="04a25-138">A chave de cada entrada é um dos usuários que a tarefa é atribuída ao e o valor é a dica de ordem.</span><span class="sxs-lookup"><span data-stu-id="04a25-138">The key of each entry is one of the users the task is assigned to and the value is the order hint.</span></span> <span data-ttu-id="04a25-139">O formato de cada valor é definido no [usando dicas de ordem no planejador (… / resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="04a25-139">The format of each value is defined in [Using order hints in Planner(../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="04a25-140">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="04a25-140">unassignedOrderHint</span></span>|<span data-ttu-id="04a25-141">String</span><span class="sxs-lookup"><span data-stu-id="04a25-141">String</span></span>|<span data-ttu-id="04a25-142">Valor de dica usado para solicitar a tarefa no modo de exibição AssignedTo da placa tarefa quando a tarefa não é atribuída a ninguém, ou se o dicionário orderHintsByAssignee não ofereça uma dica order para o usuário a tarefa é atribuída a.</span><span class="sxs-lookup"><span data-stu-id="04a25-142">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to.</span></span> <span data-ttu-id="04a25-143">O formato é definido em [dicas de ordem de uso no planejador](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="04a25-143">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="04a25-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="04a25-144">Response</span></span>

<span data-ttu-id="04a25-145">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04a25-145">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="04a25-p108">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="04a25-p108">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="04a25-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04a25-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04a25-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04a25-150">Request</span></span>
<span data-ttu-id="04a25-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04a25-151">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="04a25-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="04a25-152">Response</span></span>
<span data-ttu-id="04a25-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04a25-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerassignedtotaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
