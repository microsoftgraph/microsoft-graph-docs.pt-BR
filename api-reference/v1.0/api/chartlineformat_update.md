# <a name="update-chartlineformat"></a><span data-ttu-id="9c60f-101">Atualizar chartlineformat</span><span class="sxs-lookup"><span data-stu-id="9c60f-101">Update chartlineformat</span></span>

<span data-ttu-id="9c60f-102">Atualiza as propriedades do objeto chartlineformat.</span><span class="sxs-lookup"><span data-stu-id="9c60f-102">Update the properties of chartlineformat object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c60f-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9c60f-103">Prerequisites</span></span>
<span data-ttu-id="9c60f-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="9c60f-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="9c60f-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c60f-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="9c60f-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c60f-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/majorgridlines/format/line
```
## <a name="optional-request-headers"></a><span data-ttu-id="9c60f-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="9c60f-107">Optional request headers</span></span>
| <span data-ttu-id="9c60f-108">Nome</span><span class="sxs-lookup"><span data-stu-id="9c60f-108">Name</span></span>       | <span data-ttu-id="9c60f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c60f-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9c60f-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c60f-110">Authorization</span></span>  | <span data-ttu-id="9c60f-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c60f-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="9c60f-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c60f-113">Request body</span></span>
<span data-ttu-id="9c60f-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9c60f-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9c60f-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c60f-117">Property</span></span>     | <span data-ttu-id="9c60f-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c60f-118">Type</span></span>   |<span data-ttu-id="9c60f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c60f-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c60f-120">color</span><span class="sxs-lookup"><span data-stu-id="9c60f-120">color</span></span>|<span data-ttu-id="9c60f-121">string</span><span class="sxs-lookup"><span data-stu-id="9c60f-121">string</span></span>|<span data-ttu-id="9c60f-122">Código de cor HTML que representa a cor das linhas no gráfico.</span><span class="sxs-lookup"><span data-stu-id="9c60f-122">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="response"></a><span data-ttu-id="9c60f-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c60f-123">Response</span></span>

<span data-ttu-id="9c60f-124">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartLineFormat](../resources/chartlineformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c60f-124">If successful, this method returns a `200 OK` response code and updated [ChartLineFormat](../resources/chartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9c60f-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c60f-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c60f-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c60f-126">Request</span></span>
<span data-ttu-id="9c60f-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c60f-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlineformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="9c60f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c60f-128">Response</span></span>
<span data-ttu-id="9c60f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9c60f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartLineFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlineformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->