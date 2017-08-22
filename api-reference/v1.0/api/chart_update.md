# <a name="update-chart"></a><span data-ttu-id="c4d76-101">Atualizar gráfico</span><span class="sxs-lookup"><span data-stu-id="c4d76-101">Update chart</span></span>

<span data-ttu-id="c4d76-102">Atualiza as propriedades do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="c4d76-102">Update the properties of chart object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c4d76-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4d76-103">Prerequisites</span></span>
<span data-ttu-id="c4d76-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="c4d76-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="c4d76-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4d76-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="c4d76-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4d76-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="c4d76-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c4d76-107">Optional request headers</span></span>
| <span data-ttu-id="c4d76-108">Nome</span><span class="sxs-lookup"><span data-stu-id="c4d76-108">Name</span></span>       | <span data-ttu-id="c4d76-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4d76-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c4d76-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4d76-110">Authorization</span></span>  | <span data-ttu-id="c4d76-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4d76-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c4d76-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4d76-113">Request body</span></span>
<span data-ttu-id="c4d76-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c4d76-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c4d76-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4d76-117">Property</span></span>     | <span data-ttu-id="c4d76-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4d76-118">Type</span></span>   |<span data-ttu-id="c4d76-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4d76-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4d76-120">height</span><span class="sxs-lookup"><span data-stu-id="c4d76-120">height</span></span>|<span data-ttu-id="c4d76-121">Double</span><span class="sxs-lookup"><span data-stu-id="c4d76-121">double</span></span>|<span data-ttu-id="c4d76-122">Representa a altura, em pontos, do objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="c4d76-122">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="c4d76-123">left</span><span class="sxs-lookup"><span data-stu-id="c4d76-123">left</span></span>|<span data-ttu-id="c4d76-124">Double</span><span class="sxs-lookup"><span data-stu-id="c4d76-124">double</span></span>|<span data-ttu-id="c4d76-125">A distância, em pontos, da esquerda do gráfico à origem da planilha.</span><span class="sxs-lookup"><span data-stu-id="c4d76-125">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="c4d76-126">name</span><span class="sxs-lookup"><span data-stu-id="c4d76-126">name</span></span>|<span data-ttu-id="c4d76-127">string</span><span class="sxs-lookup"><span data-stu-id="c4d76-127">string</span></span>|<span data-ttu-id="c4d76-128">Representa o nome de um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="c4d76-128">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="c4d76-129">top</span><span class="sxs-lookup"><span data-stu-id="c4d76-129">top</span></span>|<span data-ttu-id="c4d76-130">Double</span><span class="sxs-lookup"><span data-stu-id="c4d76-130">double</span></span>|<span data-ttu-id="c4d76-131">Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="c4d76-131">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="c4d76-132">width</span><span class="sxs-lookup"><span data-stu-id="c4d76-132">width</span></span>|<span data-ttu-id="c4d76-133">Double</span><span class="sxs-lookup"><span data-stu-id="c4d76-133">double</span></span>|<span data-ttu-id="c4d76-134">Representa a largura, em pontos, do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="c4d76-134">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="c4d76-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4d76-135">Response</span></span>

<span data-ttu-id="c4d76-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Chart](../resources/chart.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4d76-136">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c4d76-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4d76-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4d76-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4d76-138">Request</span></span>
<span data-ttu-id="c4d76-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4d76-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
##### <a name="response"></a><span data-ttu-id="c4d76-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4d76-140">Response</span></span>
<span data-ttu-id="c4d76-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4d76-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->