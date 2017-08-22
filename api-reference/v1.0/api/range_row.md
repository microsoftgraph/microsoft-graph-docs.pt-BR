# <a name="range-row"></a><span data-ttu-id="5aab4-101">Range: Row</span><span class="sxs-lookup"><span data-stu-id="5aab4-101">Range: Row</span></span>

<span data-ttu-id="5aab4-102">Obtém uma linha contida no intervalo.</span><span class="sxs-lookup"><span data-stu-id="5aab4-102">Gets a row contained in the range.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5aab4-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5aab4-103">Prerequisites</span></span>
<span data-ttu-id="5aab4-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="5aab4-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="5aab4-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5aab4-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="5aab4-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5aab4-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/Row
POST /workbook/worksheets/{id|name}/range(<address>)/Row
POST /workbook/tables/{id|name}/columns/{id|name}/range/Row

```
## <a name="request-headers"></a><span data-ttu-id="5aab4-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5aab4-107">Request headers</span></span>
| <span data-ttu-id="5aab4-108">Nome</span><span class="sxs-lookup"><span data-stu-id="5aab4-108">Name</span></span>       | <span data-ttu-id="5aab4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5aab4-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5aab4-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="5aab4-110">Authorization</span></span>  | <span data-ttu-id="5aab4-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5aab4-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5aab4-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5aab4-113">Request body</span></span>
<span data-ttu-id="5aab4-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5aab4-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5aab4-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5aab4-115">Parameter</span></span>    | <span data-ttu-id="5aab4-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="5aab4-116">Type</span></span>   |<span data-ttu-id="5aab4-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="5aab4-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5aab4-118">row</span><span class="sxs-lookup"><span data-stu-id="5aab4-118">row</span></span>|<span data-ttu-id="5aab4-119">number</span><span class="sxs-lookup"><span data-stu-id="5aab4-119">number</span></span>|<span data-ttu-id="5aab4-p102">O número da linha do intervalo a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="5aab4-p102">Row number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="5aab4-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aab4-122">Response</span></span>

<span data-ttu-id="5aab4-123">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5aab4-123">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5aab4-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5aab4-124">Example</span></span>
<span data-ttu-id="5aab4-125">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5aab4-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5aab4-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5aab4-126">Request</span></span>
<span data-ttu-id="5aab4-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5aab4-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_row"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/Row
Content-type: application/json
Content-length: 18

{
  "row": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="5aab4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aab4-128">Response</span></span>
<span data-ttu-id="5aab4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5aab4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Row",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->