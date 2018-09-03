# <a name="chartcollection-add"></a><span data-ttu-id="276f6-101">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="276f6-101">ChartCollection: add</span></span>

<span data-ttu-id="276f6-102">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="276f6-102">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="276f6-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="276f6-103">Permissions</span></span>
<span data-ttu-id="276f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="276f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="276f6-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="276f6-106">Permission type</span></span>      | <span data-ttu-id="276f6-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="276f6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="276f6-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="276f6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="276f6-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="276f6-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="276f6-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="276f6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="276f6-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="276f6-111">Not supported.</span></span>    |
|<span data-ttu-id="276f6-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="276f6-112">Application</span></span> | <span data-ttu-id="276f6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="276f6-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="276f6-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="276f6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="276f6-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="276f6-115">Request headers</span></span>
| <span data-ttu-id="276f6-116">Nome</span><span class="sxs-lookup"><span data-stu-id="276f6-116">Name</span></span>       | <span data-ttu-id="276f6-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="276f6-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="276f6-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="276f6-118">Authorization</span></span>  | <span data-ttu-id="276f6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="276f6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="276f6-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="276f6-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="276f6-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="276f6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="276f6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="276f6-124">Request body</span></span>
<span data-ttu-id="276f6-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="276f6-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="276f6-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="276f6-126">Parameter</span></span>    | <span data-ttu-id="276f6-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="276f6-127">Type</span></span>   |<span data-ttu-id="276f6-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="276f6-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="276f6-129">type</span><span class="sxs-lookup"><span data-stu-id="276f6-129">type</span></span>|<span data-ttu-id="276f6-130">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="276f6-130">string</span></span>|<span data-ttu-id="276f6-131">Representa o tipo de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="276f6-131">Represents the name of a chart object.</span></span>  <span data-ttu-id="276f6-132">Os valores possíveis são: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span><span class="sxs-lookup"><span data-stu-id="276f6-132">The possible values are `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, or `PieOfPie`.</span></span>|
|<span data-ttu-id="276f6-133">sourceData</span><span class="sxs-lookup"><span data-stu-id="276f6-133">sourceData</span></span>|<span data-ttu-id="276f6-134">Json</span><span class="sxs-lookup"><span data-stu-id="276f6-134">Json</span></span>|<span data-ttu-id="276f6-135">O objeto Range que corresponde aos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="276f6-135">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="276f6-136">seriesBy</span><span class="sxs-lookup"><span data-stu-id="276f6-136">seriesBy</span></span>|<span data-ttu-id="276f6-137">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="276f6-137">string</span></span>|<span data-ttu-id="276f6-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="276f6-138">Optional.</span></span> <span data-ttu-id="276f6-139">Especifica a maneira como colunas ou linhas são usadas como série de dados no gráfico.</span><span class="sxs-lookup"><span data-stu-id="276f6-139">Returns or sets the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="276f6-140">Os valores possíveis são: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="276f6-140">The possible values are:</span></span>|

## <a name="response"></a><span data-ttu-id="276f6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="276f6-141">Response</span></span>

<span data-ttu-id="276f6-142">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [WorkbookChart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="276f6-142">If successful, this method returns `200 OK` response code and [groupSetting](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="276f6-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="276f6-143">Example</span></span>
<span data-ttu-id="276f6-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="276f6-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="276f6-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="276f6-145">Request</span></span>
<span data-ttu-id="276f6-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="276f6-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```

##### <a name="response"></a><span data-ttu-id="276f6-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="276f6-147">Response</span></span>
<span data-ttu-id="276f6-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="276f6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
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
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
