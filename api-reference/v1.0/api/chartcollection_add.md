# <a name="chartcollection-add"></a><span data-ttu-id="f91e1-101">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="f91e1-101">ChartCollection: add</span></span>

<span data-ttu-id="f91e1-102">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="f91e1-102">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="f91e1-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="f91e1-103">Permissions</span></span>
<span data-ttu-id="f91e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f91e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f91e1-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f91e1-106">Permission type</span></span>      | <span data-ttu-id="f91e1-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f91e1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f91e1-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f91e1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f91e1-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f91e1-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f91e1-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f91e1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f91e1-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f91e1-111">Not supported.</span></span>    |
|<span data-ttu-id="f91e1-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f91e1-112">Application</span></span> | <span data-ttu-id="f91e1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f91e1-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f91e1-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f91e1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="f91e1-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f91e1-115">Request headers</span></span>
| <span data-ttu-id="f91e1-116">Nome</span><span class="sxs-lookup"><span data-stu-id="f91e1-116">Name</span></span>       | <span data-ttu-id="f91e1-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f91e1-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f91e1-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="f91e1-118">Authorization</span></span>  | <span data-ttu-id="f91e1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f91e1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f91e1-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f91e1-121">Request body</span></span>
<span data-ttu-id="f91e1-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f91e1-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f91e1-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f91e1-123">Parameter</span></span>    | <span data-ttu-id="f91e1-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f91e1-124">Type</span></span>   |<span data-ttu-id="f91e1-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f91e1-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f91e1-126">type</span><span class="sxs-lookup"><span data-stu-id="f91e1-126">type</span></span>|<span data-ttu-id="f91e1-127">string</span><span class="sxs-lookup"><span data-stu-id="f91e1-127">string</span></span>|<span data-ttu-id="f91e1-p103">Representa o tipo de um gráfico.  Os valores possíveis são: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie` e `etc.`.</span><span class="sxs-lookup"><span data-stu-id="f91e1-p103">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="f91e1-130">sourceData</span><span class="sxs-lookup"><span data-stu-id="f91e1-130">sourceData</span></span>|<span data-ttu-id="f91e1-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f91e1-131">string</span></span>|<span data-ttu-id="f91e1-132">O objeto Range que corresponde aos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="f91e1-132">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="f91e1-133">seriesBy</span><span class="sxs-lookup"><span data-stu-id="f91e1-133">seriesBy</span></span>|<span data-ttu-id="f91e1-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f91e1-134">string</span></span>|<span data-ttu-id="f91e1-p104">Opcional. Especifica a forma como as colunas ou linhas são usadas como séries de dados no gráfico.  Os valores possíveis são: `Auto`, `Columns` e `Rows`.</span><span class="sxs-lookup"><span data-stu-id="f91e1-p104">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="f91e1-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f91e1-138">Response</span></span>

<span data-ttu-id="f91e1-139">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Chart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f91e1-139">If successful, this method returns `200, OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f91e1-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f91e1-140">Example</span></span>
<span data-ttu-id="f91e1-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f91e1-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f91e1-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f91e1-142">Request</span></span>
<span data-ttu-id="f91e1-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f91e1-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f91e1-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f91e1-144">Response</span></span>
<span data-ttu-id="f91e1-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f91e1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
