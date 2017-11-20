# <a name="chartcollection-add"></a><span data-ttu-id="8a056-101">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="8a056-101">ChartCollection: add</span></span>

<span data-ttu-id="8a056-102">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="8a056-102">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="8a056-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a056-103">Permissions</span></span>
<span data-ttu-id="8a056-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8a056-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8a056-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a056-106">Permission type</span></span>      | <span data-ttu-id="8a056-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a056-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a056-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a056-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8a056-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a056-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8a056-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a056-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a056-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a056-111">Not supported.</span></span>    |
|<span data-ttu-id="8a056-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a056-112">Application</span></span> | <span data-ttu-id="8a056-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a056-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a056-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a056-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="8a056-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a056-115">Request headers</span></span>
| <span data-ttu-id="8a056-116">Nome</span><span class="sxs-lookup"><span data-stu-id="8a056-116">Name</span></span>       | <span data-ttu-id="8a056-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a056-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8a056-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a056-118">Authorization</span></span>  | <span data-ttu-id="8a056-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a056-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8a056-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8a056-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="8a056-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="8a056-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a056-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a056-124">Request body</span></span>
<span data-ttu-id="8a056-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a056-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8a056-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8a056-126">Parameter</span></span>    | <span data-ttu-id="8a056-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a056-127">Type</span></span>   |<span data-ttu-id="8a056-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a056-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a056-129">type</span><span class="sxs-lookup"><span data-stu-id="8a056-129">type</span></span>|<span data-ttu-id="8a056-130">string</span><span class="sxs-lookup"><span data-stu-id="8a056-130">string</span></span>|<span data-ttu-id="8a056-p104">Representa o tipo de um gráfico.  Os valores possíveis são: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie` e `etc.`.</span><span class="sxs-lookup"><span data-stu-id="8a056-p104">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="8a056-133">sourceData</span><span class="sxs-lookup"><span data-stu-id="8a056-133">sourceData</span></span>|<span data-ttu-id="8a056-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a056-134">string</span></span>|<span data-ttu-id="8a056-135">O objeto Range que corresponde aos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="8a056-135">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="8a056-136">seriesBy</span><span class="sxs-lookup"><span data-stu-id="8a056-136">seriesBy</span></span>|<span data-ttu-id="8a056-137">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a056-137">string</span></span>|<span data-ttu-id="8a056-p105">Opcional. Especifica a forma como as colunas ou linhas são usadas como séries de dados no gráfico.  Os valores possíveis são: `Auto`, `Columns` e `Rows`.</span><span class="sxs-lookup"><span data-stu-id="8a056-p105">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="8a056-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a056-141">Response</span></span>

<span data-ttu-id="8a056-142">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Chart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a056-142">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a056-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a056-143">Example</span></span>
<span data-ttu-id="8a056-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8a056-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8a056-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a056-145">Request</span></span>
<span data-ttu-id="8a056-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a056-146">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="8a056-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a056-147">Response</span></span>
<span data-ttu-id="8a056-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a056-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
