# <a name="update-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="c2176-101">Atualizar plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c2176-101">Update plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="c2176-102">Atualize as propriedades do objeto **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="c2176-102">Update the properties of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c2176-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c2176-103">Prerequisites</span></span>
<span data-ttu-id="c2176-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="c2176-104">The following **scopes** are required to execute this API:</span></span> 

<span data-ttu-id="c2176-105">*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="c2176-105">*Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="c2176-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2176-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/bucketTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="c2176-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c2176-107">Optional request headers</span></span>
| <span data-ttu-id="c2176-108">Nome</span><span class="sxs-lookup"><span data-stu-id="c2176-108">Name</span></span>       | <span data-ttu-id="c2176-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2176-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c2176-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2176-110">Authorization</span></span>  | <span data-ttu-id="c2176-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2176-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2176-113">If-Match</span><span class="sxs-lookup"><span data-stu-id="c2176-113">If-Match</span></span>  | <span data-ttu-id="c2176-p102">Último valor ETag conhecido do objeto **plannerBucketTaskBoardTaskFormat** a ser atualizado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2176-p102">Last known ETag value for the **plannerBucketTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2176-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2176-116">Request body</span></span>
<span data-ttu-id="c2176-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c2176-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c2176-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2176-120">Property</span></span>     | <span data-ttu-id="c2176-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2176-121">Type</span></span>   |<span data-ttu-id="c2176-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2176-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2176-123">orderHint</span><span class="sxs-lookup"><span data-stu-id="c2176-123">orderHint</span></span>|<span data-ttu-id="c2176-124">String</span><span class="sxs-lookup"><span data-stu-id="c2176-124">String</span></span>|<span data-ttu-id="c2176-p104">Dica usada para ordenar tarefas no modo de exibição Bucket do Quadro de Tarefas. O formato é definido como descrito [aqui](../resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="c2176-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="c2176-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2176-127">Response</span></span>

<span data-ttu-id="c2176-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2176-128">If successful, this method returns a `200 OK` response code and updated [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="c2176-p105">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="c2176-p105">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c2176-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2176-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2176-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2176-133">Request</span></span>
<span data-ttu-id="c2176-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2176-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbuckettaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/bucketTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
##### <a name="response"></a><span data-ttu-id="c2176-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2176-135">Response</span></span>
<span data-ttu-id="c2176-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2176-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 68

{
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "orderHint": "C3665D"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerbuckettaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->