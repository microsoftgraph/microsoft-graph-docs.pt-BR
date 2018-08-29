# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="a9d50-101">Atualizar plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="a9d50-101">Update plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="a9d50-102">Atualize as propriedades do objeto **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="a9d50-102">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9d50-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9d50-103">Permissions</span></span>
<span data-ttu-id="a9d50-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a9d50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a9d50-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9d50-106">Permission type</span></span>      | <span data-ttu-id="a9d50-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9d50-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9d50-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9d50-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a9d50-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9d50-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a9d50-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9d50-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9d50-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9d50-111">Not supported.</span></span>    |
|<span data-ttu-id="a9d50-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9d50-112">Application</span></span> | <span data-ttu-id="a9d50-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9d50-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9d50-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9d50-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="a9d50-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="a9d50-115">Optional request headers</span></span>
| <span data-ttu-id="a9d50-116">Nome</span><span class="sxs-lookup"><span data-stu-id="a9d50-116">Name</span></span>       | <span data-ttu-id="a9d50-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9d50-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a9d50-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9d50-118">Authorization</span></span>  | <span data-ttu-id="a9d50-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9d50-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a9d50-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="a9d50-121">If-Match</span></span>  | <span data-ttu-id="a9d50-p103">Último valor ETag conhecido do objeto **plannerAssignedToTaskBoardTaskFormat** a ser atualizado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9d50-p103">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9d50-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9d50-124">Request body</span></span>
<span data-ttu-id="a9d50-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a9d50-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a9d50-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9d50-128">Property</span></span>     | <span data-ttu-id="a9d50-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9d50-129">Type</span></span>   |<span data-ttu-id="a9d50-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9d50-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9d50-131">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="a9d50-131">orderHintsByAssignee</span></span>|[<span data-ttu-id="a9d50-132">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="a9d50-132">plannerOrderHintsByAssignee</span></span>](../resources/plannerOrderHintsByAssignee.md)|<span data-ttu-id="a9d50-p105">O dicionário de dicas usado para ordenar tarefas no modo de exibição AssignedTo do Quadro de Tarefas. A chave de cada entrada é um dos usuários ao qual a tarefa é atribuída, e o valor é a dica de ordem. O formato de cada valor é definido como descrito [aqui](../resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="a9d50-p105">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="a9d50-136">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="a9d50-136">unassignedOrderHint</span></span>|<span data-ttu-id="a9d50-137">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9d50-137">String</span></span>|<span data-ttu-id="a9d50-p106">Valor da dica usado para ordenar a tarefa no modo de exibição AssignedTo do Quadro de Tarefas quando a tarefa não for atribuída a ninguém ou se o dicionário orderHintsByAssignee não oferecer uma dica de ordem para o usuário à qual a tarefa foi atribuída. O formato é definido como descrito [aqui](../resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="a9d50-p106">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="a9d50-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9d50-140">Response</span></span>

<span data-ttu-id="a9d50-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9d50-141">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="a9d50-p107">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="a9d50-p107">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="a9d50-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9d50-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9d50-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9d50-146">Request</span></span>
<span data-ttu-id="a9d50-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9d50-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/assignedToTaskBoardFormat
Content-type: application/json
Content-length: 96
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHintsByAssignee": {
    "aaa27244-1db4-476a-a5cb-004607466324": "8566473P 957764Jk!"
  }
}
```
##### <a name="response"></a><span data-ttu-id="a9d50-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9d50-148">Response</span></span>
<span data-ttu-id="a9d50-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9d50-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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