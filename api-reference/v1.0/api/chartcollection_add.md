# <a name="chartcollection-add"></a><span data-ttu-id="0e7e8-101">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="0e7e8-101">ChartCollection: add</span></span>

<span data-ttu-id="0e7e8-102">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="0e7e8-102">Creates a new chart.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0e7e8-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0e7e8-103">Prerequisites</span></span>
<span data-ttu-id="0e7e8-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="0e7e8-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="0e7e8-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e7e8-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="0e7e8-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e7e8-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="0e7e8-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e7e8-107">Request headers</span></span>
| <span data-ttu-id="0e7e8-108">Nome</span><span class="sxs-lookup"><span data-stu-id="0e7e8-108">Name</span></span>       | <span data-ttu-id="0e7e8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e7e8-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0e7e8-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e7e8-110">Authorization</span></span>  | <span data-ttu-id="0e7e8-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e7e8-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0e7e8-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e7e8-113">Request body</span></span>
<span data-ttu-id="0e7e8-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e7e8-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0e7e8-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0e7e8-115">Parameter</span></span>    | <span data-ttu-id="0e7e8-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e7e8-116">Type</span></span>   |<span data-ttu-id="0e7e8-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e7e8-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e7e8-118">type</span><span class="sxs-lookup"><span data-stu-id="0e7e8-118">type</span></span>|<span data-ttu-id="0e7e8-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e7e8-119">string</span></span>|<span data-ttu-id="0e7e8-p102">Representa o tipo de um gráfico.  Os valores possíveis são: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie` e `etc.`.</span><span class="sxs-lookup"><span data-stu-id="0e7e8-p102">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="0e7e8-122">sourceData</span><span class="sxs-lookup"><span data-stu-id="0e7e8-122">sourceData</span></span>|<span data-ttu-id="0e7e8-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e7e8-123">string</span></span>|<span data-ttu-id="0e7e8-124">O objeto Range que corresponde aos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="0e7e8-124">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="0e7e8-125">seriesBy</span><span class="sxs-lookup"><span data-stu-id="0e7e8-125">seriesBy</span></span>|<span data-ttu-id="0e7e8-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e7e8-126">string</span></span>|<span data-ttu-id="0e7e8-p103">Opcional. Especifica a forma como as colunas ou linhas são usadas como séries de dados no gráfico.  Os valores possíveis são: `Auto`, `Columns` e `Rows`.</span><span class="sxs-lookup"><span data-stu-id="0e7e8-p103">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="0e7e8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e7e8-130">Response</span></span>

<span data-ttu-id="0e7e8-131">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Chart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e7e8-131">If successful, this method returns `200, OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e7e8-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e7e8-132">Example</span></span>
<span data-ttu-id="0e7e8-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0e7e8-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0e7e8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e7e8-134">Request</span></span>
<span data-ttu-id="0e7e8-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e7e8-135">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="0e7e8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e7e8-136">Response</span></span>
<span data-ttu-id="0e7e8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e7e8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
