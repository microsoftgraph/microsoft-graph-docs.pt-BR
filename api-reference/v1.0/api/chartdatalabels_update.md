# <a name="update-chartdatalabels"></a><span data-ttu-id="47457-101">Atualizar chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="47457-101">Update chartdatalabels</span></span>

<span data-ttu-id="47457-102">Atualiza as propriedades do objeto chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="47457-102">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="47457-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="47457-103">Permissions</span></span>
<span data-ttu-id="47457-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="47457-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="47457-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47457-106">Permission type</span></span>      | <span data-ttu-id="47457-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47457-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47457-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47457-108">Delegated (work or school account)</span></span> | <span data-ttu-id="47457-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47457-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="47457-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47457-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47457-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47457-111">Not supported.</span></span>    |
|<span data-ttu-id="47457-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47457-112">Application</span></span> | <span data-ttu-id="47457-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47457-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="47457-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47457-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="47457-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="47457-115">Optional request headers</span></span>
| <span data-ttu-id="47457-116">Nome</span><span class="sxs-lookup"><span data-stu-id="47457-116">Name</span></span>       | <span data-ttu-id="47457-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="47457-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="47457-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="47457-118">Authorization</span></span>  | <span data-ttu-id="47457-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47457-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47457-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47457-121">Request body</span></span>
<span data-ttu-id="47457-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="47457-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="47457-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47457-125">Property</span></span>     | <span data-ttu-id="47457-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="47457-126">Type</span></span>   |<span data-ttu-id="47457-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="47457-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47457-128">position</span><span class="sxs-lookup"><span data-stu-id="47457-128">position</span></span>|<span data-ttu-id="47457-129">string</span><span class="sxs-lookup"><span data-stu-id="47457-129">string</span></span>|<span data-ttu-id="47457-p104">Valor de DataLabelPosition que representa a posição do rótulo de dados. Os valores possíveis são: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit` e `Callout`.</span><span class="sxs-lookup"><span data-stu-id="47457-p104">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="47457-132">separador</span><span class="sxs-lookup"><span data-stu-id="47457-132">separator</span></span>|<span data-ttu-id="47457-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47457-133">string</span></span>|<span data-ttu-id="47457-134">Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="47457-134">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="47457-135">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="47457-135">showBubbleSize</span></span>|<span data-ttu-id="47457-136">booliano</span><span class="sxs-lookup"><span data-stu-id="47457-136">boolean</span></span>|<span data-ttu-id="47457-137">Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="47457-137">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="47457-138">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="47457-138">showCategoryName</span></span>|<span data-ttu-id="47457-139">booliano</span><span class="sxs-lookup"><span data-stu-id="47457-139">boolean</span></span>|<span data-ttu-id="47457-140">Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="47457-140">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="47457-141">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="47457-141">showLegendKey</span></span>|<span data-ttu-id="47457-142">booliano</span><span class="sxs-lookup"><span data-stu-id="47457-142">boolean</span></span>|<span data-ttu-id="47457-143">Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="47457-143">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="47457-144">showPercentage</span><span class="sxs-lookup"><span data-stu-id="47457-144">showPercentage</span></span>|<span data-ttu-id="47457-145">booliano</span><span class="sxs-lookup"><span data-stu-id="47457-145">boolean</span></span>|<span data-ttu-id="47457-146">Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="47457-146">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="47457-147">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="47457-147">showSeriesName</span></span>|<span data-ttu-id="47457-148">booliano</span><span class="sxs-lookup"><span data-stu-id="47457-148">boolean</span></span>|<span data-ttu-id="47457-149">Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="47457-149">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="47457-150">showValue</span><span class="sxs-lookup"><span data-stu-id="47457-150">showValue</span></span>|<span data-ttu-id="47457-151">booliano</span><span class="sxs-lookup"><span data-stu-id="47457-151">boolean</span></span>|<span data-ttu-id="47457-152">Valor booliano que determina se o valor do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="47457-152">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="47457-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="47457-153">Response</span></span>

<span data-ttu-id="47457-154">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartDataLabels](../resources/chartdatalabels.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47457-154">If successful, this method returns a `200 OK` response code and updated [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="47457-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47457-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47457-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47457-156">Request</span></span>
<span data-ttu-id="47457-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47457-157">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="47457-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="47457-158">Response</span></span>
<span data-ttu-id="47457-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47457-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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