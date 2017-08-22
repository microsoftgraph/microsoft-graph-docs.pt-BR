# <a name="update-plannerbucket"></a><span data-ttu-id="c28d4-101">Atualizar plannerbucket</span><span class="sxs-lookup"><span data-stu-id="c28d4-101">Update plannerbucket</span></span>

<span data-ttu-id="c28d4-102">Atualize as propriedades do objeto **plannerbucket**.</span><span class="sxs-lookup"><span data-stu-id="c28d4-102">Update the properties of **plannerbucket** object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c28d4-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c28d4-103">Prerequisites</span></span>
<span data-ttu-id="c28d4-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="c28d4-104">The following **scopes** are required to execute this API:</span></span> 

<span data-ttu-id="c28d4-105">*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="c28d4-105">*Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="c28d4-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c28d4-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="c28d4-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c28d4-107">Optional request headers</span></span>
| <span data-ttu-id="c28d4-108">Nome</span><span class="sxs-lookup"><span data-stu-id="c28d4-108">Name</span></span>       | <span data-ttu-id="c28d4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c28d4-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c28d4-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="c28d4-110">Authorization</span></span>  | <span data-ttu-id="c28d4-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c28d4-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c28d4-113">If-Match</span><span class="sxs-lookup"><span data-stu-id="c28d4-113">If-Match</span></span>  | <span data-ttu-id="c28d4-p102">O último valor ETag conhecido do objeto **plannerBucket** a ser atualizado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c28d4-p102">Last known ETag value for the **plannerBucket** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c28d4-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c28d4-116">Request body</span></span>
<span data-ttu-id="c28d4-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c28d4-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c28d4-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c28d4-120">Property</span></span>     | <span data-ttu-id="c28d4-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c28d4-121">Type</span></span>   |<span data-ttu-id="c28d4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c28d4-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c28d4-123">name</span><span class="sxs-lookup"><span data-stu-id="c28d4-123">name</span></span>|<span data-ttu-id="c28d4-124">String</span><span class="sxs-lookup"><span data-stu-id="c28d4-124">String</span></span>|<span data-ttu-id="c28d4-125">Nome do bucket.</span><span class="sxs-lookup"><span data-stu-id="c28d4-125">Name of the bucket.</span></span>|
|<span data-ttu-id="c28d4-126">orderHint</span><span class="sxs-lookup"><span data-stu-id="c28d4-126">orderHint</span></span>|<span data-ttu-id="c28d4-127">String</span><span class="sxs-lookup"><span data-stu-id="c28d4-127">String</span></span>|<span data-ttu-id="c28d4-p104">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](../resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="c28d4-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="c28d4-130">planId</span><span class="sxs-lookup"><span data-stu-id="c28d4-130">planId</span></span>|<span data-ttu-id="c28d4-131">String</span><span class="sxs-lookup"><span data-stu-id="c28d4-131">String</span></span>|<span data-ttu-id="c28d4-132">ID do plano ao qual o bucket pertence.</span><span class="sxs-lookup"><span data-stu-id="c28d4-132">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="c28d4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c28d4-133">Response</span></span>

<span data-ttu-id="c28d4-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerBucket](../resources/plannerbucket.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c28d4-134">If successful, this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="c28d4-p105">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="c28d4-p105">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c28d4-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c28d4-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c28d4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c28d4-139">Request</span></span>
<span data-ttu-id="c28d4-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c28d4-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbucket"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/buckets/hsOf2dhOJkqyYYZEtdzDe2QAIUCR
Content-type: application/json
Content-length: 27
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "name": "Development"
}
```
##### <a name="response"></a><span data-ttu-id="c28d4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c28d4-141">Response</span></span>
<span data-ttu-id="c28d4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c28d4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "name": "Development",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerbucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->