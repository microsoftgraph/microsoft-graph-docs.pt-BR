# <a name="range-cell"></a><span data-ttu-id="af144-101">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="af144-101">Range: Cell</span></span>

<span data-ttu-id="af144-p101">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha. A localização da célula retornada está relacionada à célula superior esquerda do intervalo.</span><span class="sxs-lookup"><span data-stu-id="af144-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af144-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="af144-105">Prerequisites</span></span>
<span data-ttu-id="af144-106">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="af144-106">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="af144-107">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af144-107">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="af144-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af144-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Cell
GET /workbook/worksheets/{id|name}/range(<address>)/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="af144-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af144-109">Request headers</span></span>
| <span data-ttu-id="af144-110">Nome</span><span class="sxs-lookup"><span data-stu-id="af144-110">Name</span></span>       | <span data-ttu-id="af144-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="af144-111">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="af144-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="af144-112">Authorization</span></span>  | <span data-ttu-id="af144-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af144-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="af144-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af144-115">Request body</span></span>
<span data-ttu-id="af144-116">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af144-116">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="af144-117">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="af144-117">Parameter</span></span>    | <span data-ttu-id="af144-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="af144-118">Type</span></span>   |<span data-ttu-id="af144-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="af144-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af144-120">row</span><span class="sxs-lookup"><span data-stu-id="af144-120">row</span></span>|<span data-ttu-id="af144-121">number</span><span class="sxs-lookup"><span data-stu-id="af144-121">number</span></span>|<span data-ttu-id="af144-p103">O número da linha da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="af144-p103">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="af144-124">column</span><span class="sxs-lookup"><span data-stu-id="af144-124">column</span></span>|<span data-ttu-id="af144-125">number</span><span class="sxs-lookup"><span data-stu-id="af144-125">number</span></span>|<span data-ttu-id="af144-p104">O número da coluna da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="af144-p104">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="af144-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="af144-128">Response</span></span>

<span data-ttu-id="af144-129">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af144-129">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af144-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af144-130">Example</span></span>
<span data-ttu-id="af144-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="af144-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="af144-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af144-132">Request</span></span>
<span data-ttu-id="af144-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af144-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/Cell
Content-type: application/json
Content-length: 37

{
  "row": {
  },
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="af144-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="af144-134">Response</span></span>
<span data-ttu-id="af144-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af144-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->