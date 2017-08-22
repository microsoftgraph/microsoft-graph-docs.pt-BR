# <a name="range-insert"></a><span data-ttu-id="58866-101">Range: insert</span><span class="sxs-lookup"><span data-stu-id="58866-101">Range: insert</span></span>

<span data-ttu-id="58866-p101">Insere uma célula ou um intervalo de células na planilha, no lugar desse intervalo, e desloca as outras células para liberar espaço. Retorna um novo objeto Range no espaço em branco atual.</span><span class="sxs-lookup"><span data-stu-id="58866-p101">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58866-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58866-104">Prerequisites</span></span>
<span data-ttu-id="58866-105">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="58866-105">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="58866-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58866-106">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="58866-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58866-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/insert
POST /workbook/worksheets/{id|name}/range(<address>)/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="58866-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58866-108">Request headers</span></span>
| <span data-ttu-id="58866-109">Nome</span><span class="sxs-lookup"><span data-stu-id="58866-109">Name</span></span>       | <span data-ttu-id="58866-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="58866-110">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="58866-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="58866-111">Authorization</span></span>  | <span data-ttu-id="58866-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58866-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="58866-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58866-114">Request body</span></span>
<span data-ttu-id="58866-115">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58866-115">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="58866-116">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="58866-116">Parameter</span></span>    | <span data-ttu-id="58866-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="58866-117">Type</span></span>   |<span data-ttu-id="58866-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="58866-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58866-119">shift</span><span class="sxs-lookup"><span data-stu-id="58866-119">shift</span></span>|<span data-ttu-id="58866-120">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58866-120">string</span></span>|<span data-ttu-id="58866-p103">Especifica como deslocar as células.  Os valores possíveis são: `Down` e `Right`.</span><span class="sxs-lookup"><span data-stu-id="58866-p103">Specifies which way to shift the cells.  Possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="58866-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="58866-123">Response</span></span>

<span data-ttu-id="58866-124">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58866-124">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58866-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58866-125">Example</span></span>
<span data-ttu-id="58866-126">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="58866-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="58866-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58866-127">Request</span></span>
<span data-ttu-id="58866-128">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58866-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="58866-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="58866-129">Response</span></span>
<span data-ttu-id="58866-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58866-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->