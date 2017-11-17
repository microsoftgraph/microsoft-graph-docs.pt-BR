# <a name="range-cell"></a><span data-ttu-id="e9393-101">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="e9393-101">Range: Cell</span></span>

<span data-ttu-id="e9393-p101">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha. A localização da célula retornada está relacionada à célula superior esquerda do intervalo.</span><span class="sxs-lookup"><span data-stu-id="e9393-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="e9393-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9393-105">Permissions</span></span>
<span data-ttu-id="e9393-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e9393-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e9393-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9393-108">Permission type</span></span>      | <span data-ttu-id="e9393-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9393-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9393-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9393-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e9393-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9393-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e9393-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9393-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9393-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9393-113">Not supported.</span></span>    |
|<span data-ttu-id="e9393-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9393-114">Application</span></span> | <span data-ttu-id="e9393-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9393-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9393-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9393-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="e9393-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9393-117">Request headers</span></span>
| <span data-ttu-id="e9393-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e9393-118">Name</span></span>       | <span data-ttu-id="e9393-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9393-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e9393-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9393-120">Authorization</span></span>  | <span data-ttu-id="e9393-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9393-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9393-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9393-123">Request body</span></span>
<span data-ttu-id="e9393-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9393-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e9393-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e9393-125">Parameter</span></span>    | <span data-ttu-id="e9393-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9393-126">Type</span></span>   |<span data-ttu-id="e9393-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9393-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9393-128">row</span><span class="sxs-lookup"><span data-stu-id="e9393-128">row</span></span>|<span data-ttu-id="e9393-129">number</span><span class="sxs-lookup"><span data-stu-id="e9393-129">number</span></span>|<span data-ttu-id="e9393-p104">O número da linha da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="e9393-p104">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="e9393-132">column</span><span class="sxs-lookup"><span data-stu-id="e9393-132">column</span></span>|<span data-ttu-id="e9393-133">number</span><span class="sxs-lookup"><span data-stu-id="e9393-133">number</span></span>|<span data-ttu-id="e9393-p105">O número da coluna da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="e9393-p105">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="e9393-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9393-136">Response</span></span>

<span data-ttu-id="e9393-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9393-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9393-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9393-138">Example</span></span>
<span data-ttu-id="e9393-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e9393-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e9393-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9393-140">Request</span></span>
<span data-ttu-id="e9393-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9393-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="e9393-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9393-142">Response</span></span>
<span data-ttu-id="e9393-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9393-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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