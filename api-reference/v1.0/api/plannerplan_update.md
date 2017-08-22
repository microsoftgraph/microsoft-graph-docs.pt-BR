# <a name="update-plannerplan"></a><span data-ttu-id="0bd23-101">Atualizar plannerplan</span><span class="sxs-lookup"><span data-stu-id="0bd23-101">Update plannerplan</span></span>

<span data-ttu-id="0bd23-102">Atualize as propriedades do objeto **plannerplan**.</span><span class="sxs-lookup"><span data-stu-id="0bd23-102">Update the properties of **plannerplan** object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0bd23-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0bd23-103">Prerequisites</span></span>
<span data-ttu-id="0bd23-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="0bd23-104">The following **scopes** are required to execute this API:</span></span> 

<span data-ttu-id="0bd23-105">*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="0bd23-105">*Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="0bd23-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0bd23-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="0bd23-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="0bd23-107">Optional request headers</span></span>
| <span data-ttu-id="0bd23-108">Nome</span><span class="sxs-lookup"><span data-stu-id="0bd23-108">Name</span></span>       | <span data-ttu-id="0bd23-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bd23-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0bd23-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="0bd23-110">Authorization</span></span>  | <span data-ttu-id="0bd23-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bd23-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0bd23-113">If-Match</span><span class="sxs-lookup"><span data-stu-id="0bd23-113">If-Match</span></span>  | <span data-ttu-id="0bd23-p102">O último valor ETag conhecido do objeto plannerPlan a ser atualizado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bd23-p102">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bd23-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0bd23-116">Request body</span></span>
<span data-ttu-id="0bd23-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0bd23-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0bd23-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bd23-120">Property</span></span>     | <span data-ttu-id="0bd23-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bd23-121">Type</span></span>   |<span data-ttu-id="0bd23-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bd23-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0bd23-123">owner</span><span class="sxs-lookup"><span data-stu-id="0bd23-123">owner</span></span>|<span data-ttu-id="0bd23-124">String</span><span class="sxs-lookup"><span data-stu-id="0bd23-124">String</span></span>|<span data-ttu-id="0bd23-p104">[Grupo](../resources/group.md) `id` ao qual o plano pertence. Deve haver um grupo válido para que esse campo possa ser definido. Após definido, ele só poderá ser atualizado pelo proprietário.</span><span class="sxs-lookup"><span data-stu-id="0bd23-p104">[Group](../resources/group.md) `id` by which the plan is owned. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="0bd23-128">title</span><span class="sxs-lookup"><span data-stu-id="0bd23-128">title</span></span>|<span data-ttu-id="0bd23-129">String</span><span class="sxs-lookup"><span data-stu-id="0bd23-129">String</span></span>|<span data-ttu-id="0bd23-130">Título do plano.</span><span class="sxs-lookup"><span data-stu-id="0bd23-130">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="0bd23-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bd23-131">Response</span></span>

<span data-ttu-id="0bd23-132">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerPlan](../resources/plannerplan.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bd23-132">If successful, this method returns a `200 OK` response code and updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="0bd23-p105">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="0bd23-p105">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="0bd23-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0bd23-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0bd23-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bd23-137">Request</span></span>
<span data-ttu-id="0bd23-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bd23-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
##### <a name="response"></a><span data-ttu-id="0bd23-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bd23-139">Response</span></span>
<span data-ttu-id="0bd23-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0bd23-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->