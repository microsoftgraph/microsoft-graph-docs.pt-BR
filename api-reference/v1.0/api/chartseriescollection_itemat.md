# <a name="chartseriescollection-itemat"></a><span data-ttu-id="1a774-101">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="1a774-101">ChartSeriesCollection: ItemAt</span></span>

<span data-ttu-id="1a774-102">Recupera uma série com base na respectiva posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="1a774-102">Retrieves a series based on its position in the collection</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1a774-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1a774-103">Prerequisites</span></span>
<span data-ttu-id="1a774-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="1a774-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="1a774-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a774-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="1a774-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a774-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="1a774-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a774-107">Request headers</span></span>
| <span data-ttu-id="1a774-108">Nome</span><span class="sxs-lookup"><span data-stu-id="1a774-108">Name</span></span>       | <span data-ttu-id="1a774-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a774-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1a774-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a774-110">Authorization</span></span>  | <span data-ttu-id="1a774-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a774-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="1a774-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a774-113">Request body</span></span>
<span data-ttu-id="1a774-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a774-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1a774-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1a774-115">Parameter</span></span>    | <span data-ttu-id="1a774-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a774-116">Type</span></span>   |<span data-ttu-id="1a774-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a774-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a774-118">índice</span><span class="sxs-lookup"><span data-stu-id="1a774-118">index</span></span>|<span data-ttu-id="1a774-119">number</span><span class="sxs-lookup"><span data-stu-id="1a774-119">number</span></span>|<span data-ttu-id="1a774-p102">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="1a774-p102">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="1a774-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a774-122">Response</span></span>

<span data-ttu-id="1a774-123">Se bem-sucedido, este método retorna um código de resposta `200, OK` e um objeto [ChartSeries](../resources/chartseries.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a774-123">If successful, this method returns `200, OK` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a774-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a774-124">Example</span></span>
<span data-ttu-id="1a774-125">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1a774-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1a774-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a774-126">Request</span></span>
<span data-ttu-id="1a774-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a774-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="1a774-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a774-128">Response</span></span>
<span data-ttu-id="1a774-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a774-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->