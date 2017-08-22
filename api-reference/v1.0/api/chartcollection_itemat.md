# <a name="chartcollection-itemat"></a><span data-ttu-id="d3e3a-101">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="d3e3a-101">ChartCollection: ItemAt</span></span>

<span data-ttu-id="d3e3a-102">Obtém um gráfico com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="d3e3a-102">Gets a chart based on its position in the collection.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d3e3a-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3e3a-103">Prerequisites</span></span>
<span data-ttu-id="d3e3a-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="d3e3a-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="d3e3a-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3e3a-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="d3e3a-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3e3a-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="d3e3a-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e3a-107">Request headers</span></span>
| <span data-ttu-id="d3e3a-108">Nome</span><span class="sxs-lookup"><span data-stu-id="d3e3a-108">Name</span></span>       | <span data-ttu-id="d3e3a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3e3a-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d3e3a-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3e3a-110">Authorization</span></span>  | <span data-ttu-id="d3e3a-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3e3a-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d3e3a-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e3a-113">Request body</span></span>
<span data-ttu-id="d3e3a-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3e3a-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d3e3a-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d3e3a-115">Parameter</span></span>    | <span data-ttu-id="d3e3a-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3e3a-116">Type</span></span>   |<span data-ttu-id="d3e3a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3e3a-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3e3a-118">índice</span><span class="sxs-lookup"><span data-stu-id="d3e3a-118">index</span></span>|<span data-ttu-id="d3e3a-119">number</span><span class="sxs-lookup"><span data-stu-id="d3e3a-119">number</span></span>|<span data-ttu-id="d3e3a-p102">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="d3e3a-p102">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="d3e3a-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3e3a-122">Response</span></span>

<span data-ttu-id="d3e3a-123">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Chart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3e3a-123">If successful, this method returns `200, OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3e3a-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3e3a-124">Example</span></span>
<span data-ttu-id="d3e3a-125">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d3e3a-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d3e3a-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e3a-126">Request</span></span>
<span data-ttu-id="d3e3a-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3e3a-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="d3e3a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3e3a-128">Response</span></span>
<span data-ttu-id="d3e3a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3e3a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "ChartCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->