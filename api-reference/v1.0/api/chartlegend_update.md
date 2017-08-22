# <a name="update-chartlegend"></a><span data-ttu-id="5e4a7-101">Atualizar chartlegend</span><span class="sxs-lookup"><span data-stu-id="5e4a7-101">Update chartlegend</span></span>

<span data-ttu-id="5e4a7-102">Atualiza as propriedades do objeto chartlegend.</span><span class="sxs-lookup"><span data-stu-id="5e4a7-102">Update the properties of chartlegend object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5e4a7-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e4a7-103">Prerequisites</span></span>
<span data-ttu-id="5e4a7-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="5e4a7-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="5e4a7-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e4a7-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="5e4a7-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e4a7-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="5e4a7-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="5e4a7-107">Optional request headers</span></span>
| <span data-ttu-id="5e4a7-108">Nome</span><span class="sxs-lookup"><span data-stu-id="5e4a7-108">Name</span></span>       | <span data-ttu-id="5e4a7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e4a7-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5e4a7-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e4a7-110">Authorization</span></span>  | <span data-ttu-id="5e4a7-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e4a7-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5e4a7-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e4a7-113">Request body</span></span>
<span data-ttu-id="5e4a7-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5e4a7-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5e4a7-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e4a7-117">Property</span></span>     | <span data-ttu-id="5e4a7-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e4a7-118">Type</span></span>   |<span data-ttu-id="5e4a7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e4a7-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e4a7-120">overlay</span><span class="sxs-lookup"><span data-stu-id="5e4a7-120">overlay</span></span>|<span data-ttu-id="5e4a7-121">booliano</span><span class="sxs-lookup"><span data-stu-id="5e4a7-121">boolean</span></span>|<span data-ttu-id="5e4a7-122">Valor booliano para determinar se a legenda do gráfico deve se sobrepor ao corpo principal do gráfico.</span><span class="sxs-lookup"><span data-stu-id="5e4a7-122">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="5e4a7-123">position</span><span class="sxs-lookup"><span data-stu-id="5e4a7-123">position</span></span>|<span data-ttu-id="5e4a7-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e4a7-124">string</span></span>|<span data-ttu-id="5e4a7-p103">Representa a posição da legenda no gráfico. Os valores possíveis são: `Top`, `Bottom`, `Left`, `Right`, `Corner` e `Custom`.</span><span class="sxs-lookup"><span data-stu-id="5e4a7-p103">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="5e4a7-127">visible</span><span class="sxs-lookup"><span data-stu-id="5e4a7-127">visible</span></span>|<span data-ttu-id="5e4a7-128">booliano</span><span class="sxs-lookup"><span data-stu-id="5e4a7-128">boolean</span></span>|<span data-ttu-id="5e4a7-129">Um valor booliano que representa a visibilidade de um objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="5e4a7-129">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="5e4a7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e4a7-130">Response</span></span>

<span data-ttu-id="5e4a7-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartLegend](../resources/chartlegend.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e4a7-131">If successful, this method returns a `200 OK` response code and updated [ChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5e4a7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e4a7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e4a7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e4a7-133">Request</span></span>
<span data-ttu-id="5e4a7-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e4a7-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="5e4a7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e4a7-135">Response</span></span>
<span data-ttu-id="5e4a7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e4a7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->