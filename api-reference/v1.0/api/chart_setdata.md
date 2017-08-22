# <a name="chart-setdata"></a><span data-ttu-id="d82c9-101">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="d82c9-101">Chart: setData</span></span>

<span data-ttu-id="d82c9-102">Redefine os dados de origem do gráfico.</span><span class="sxs-lookup"><span data-stu-id="d82c9-102">Resets the source data for the chart.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d82c9-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d82c9-103">Prerequisites</span></span>
<span data-ttu-id="d82c9-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="d82c9-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="d82c9-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d82c9-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="d82c9-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d82c9-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setData

```
## <a name="request-headers"></a><span data-ttu-id="d82c9-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d82c9-107">Request headers</span></span>
| <span data-ttu-id="d82c9-108">Nome</span><span class="sxs-lookup"><span data-stu-id="d82c9-108">Name</span></span>       | <span data-ttu-id="d82c9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d82c9-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d82c9-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="d82c9-110">Authorization</span></span>  | <span data-ttu-id="d82c9-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d82c9-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d82c9-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d82c9-113">Request body</span></span>
<span data-ttu-id="d82c9-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d82c9-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d82c9-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d82c9-115">Parameter</span></span>    | <span data-ttu-id="d82c9-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="d82c9-116">Type</span></span>   |<span data-ttu-id="d82c9-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="d82c9-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d82c9-118">sourceData</span><span class="sxs-lookup"><span data-stu-id="d82c9-118">sourceData</span></span>|<span data-ttu-id="d82c9-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82c9-119">string</span></span>|<span data-ttu-id="d82c9-120">O objeto Range que corresponde aos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="d82c9-120">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="d82c9-121">seriesBy</span><span class="sxs-lookup"><span data-stu-id="d82c9-121">seriesBy</span></span>|<span data-ttu-id="d82c9-122">string</span><span class="sxs-lookup"><span data-stu-id="d82c9-122">string</span></span>|<span data-ttu-id="d82c9-p102">Opcional. Especifica a forma como as colunas ou linhas são usadas como série de dados no gráfico. Pode ser um dos seguintes: automático (padrão), linhas ou colunas.  Os valores possíveis são: `Auto`, `Columns` e `Rows`.</span><span class="sxs-lookup"><span data-stu-id="d82c9-p102">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="d82c9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d82c9-127">Response</span></span>

<span data-ttu-id="d82c9-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d82c9-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d82c9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d82c9-130">Example</span></span>
<span data-ttu-id="d82c9-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d82c9-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d82c9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d82c9-132">Request</span></span>
<span data-ttu-id="d82c9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d82c9-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="d82c9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d82c9-134">Response</span></span>
<span data-ttu-id="d82c9-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d82c9-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->