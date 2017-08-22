# <a name="update-chartdatalabels"></a><span data-ttu-id="1e31c-101">Atualizar chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="1e31c-101">Update chartdatalabels</span></span>

<span data-ttu-id="1e31c-102">Atualiza as propriedades do objeto chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="1e31c-102">Update the properties of chartdatalabels object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e31c-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e31c-103">Prerequisites</span></span>
<span data-ttu-id="1e31c-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="1e31c-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="1e31c-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e31c-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="1e31c-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e31c-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="1e31c-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="1e31c-107">Optional request headers</span></span>
| <span data-ttu-id="1e31c-108">Nome</span><span class="sxs-lookup"><span data-stu-id="1e31c-108">Name</span></span>       | <span data-ttu-id="1e31c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e31c-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1e31c-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e31c-110">Authorization</span></span>  | <span data-ttu-id="1e31c-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e31c-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="1e31c-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e31c-113">Request body</span></span>
<span data-ttu-id="1e31c-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1e31c-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1e31c-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e31c-117">Property</span></span>     | <span data-ttu-id="1e31c-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e31c-118">Type</span></span>   |<span data-ttu-id="1e31c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e31c-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e31c-120">position</span><span class="sxs-lookup"><span data-stu-id="1e31c-120">position</span></span>|<span data-ttu-id="1e31c-121">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e31c-121">string</span></span>|<span data-ttu-id="1e31c-p103">Valor de DataLabelPosition que representa a posição do rótulo de dados. Os valores possíveis são: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit` e `Callout`.</span><span class="sxs-lookup"><span data-stu-id="1e31c-p103">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="1e31c-124">separator</span><span class="sxs-lookup"><span data-stu-id="1e31c-124">separator</span></span>|<span data-ttu-id="1e31c-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e31c-125">string</span></span>|<span data-ttu-id="1e31c-126">Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="1e31c-126">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="1e31c-127">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="1e31c-127">showBubbleSize</span></span>|<span data-ttu-id="1e31c-128">booliano</span><span class="sxs-lookup"><span data-stu-id="1e31c-128">boolean</span></span>|<span data-ttu-id="1e31c-129">Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="1e31c-129">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="1e31c-130">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="1e31c-130">showCategoryName</span></span>|<span data-ttu-id="1e31c-131">booliano</span><span class="sxs-lookup"><span data-stu-id="1e31c-131">boolean</span></span>|<span data-ttu-id="1e31c-132">Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="1e31c-132">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="1e31c-133">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="1e31c-133">showLegendKey</span></span>|<span data-ttu-id="1e31c-134">booliano</span><span class="sxs-lookup"><span data-stu-id="1e31c-134">boolean</span></span>|<span data-ttu-id="1e31c-135">Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="1e31c-135">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="1e31c-136">showPercentage</span><span class="sxs-lookup"><span data-stu-id="1e31c-136">showPercentage</span></span>|<span data-ttu-id="1e31c-137">booliano</span><span class="sxs-lookup"><span data-stu-id="1e31c-137">boolean</span></span>|<span data-ttu-id="1e31c-138">Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="1e31c-138">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="1e31c-139">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="1e31c-139">showSeriesName</span></span>|<span data-ttu-id="1e31c-140">booliano</span><span class="sxs-lookup"><span data-stu-id="1e31c-140">boolean</span></span>|<span data-ttu-id="1e31c-141">Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="1e31c-141">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="1e31c-142">showValue</span><span class="sxs-lookup"><span data-stu-id="1e31c-142">showValue</span></span>|<span data-ttu-id="1e31c-143">booliano</span><span class="sxs-lookup"><span data-stu-id="1e31c-143">boolean</span></span>|<span data-ttu-id="1e31c-144">Valor booliano que determina se o valor do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="1e31c-144">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="1e31c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e31c-145">Response</span></span>

<span data-ttu-id="1e31c-146">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartDataLabels](../resources/chartdatalabels.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e31c-146">If successful, this method returns a `200 OK` response code and updated [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1e31c-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e31c-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e31c-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e31c-148">Request</span></span>
<span data-ttu-id="1e31c-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e31c-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/datalabels
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```
##### <a name="response"></a><span data-ttu-id="1e31c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e31c-150">Response</span></span>
<span data-ttu-id="1e31c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e31c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartDataLabels"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->