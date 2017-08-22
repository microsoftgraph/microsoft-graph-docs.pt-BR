# <a name="range-offsetrange"></a><span data-ttu-id="2d97d-101">Range: OffsetRange</span><span class="sxs-lookup"><span data-stu-id="2d97d-101">Range: OffsetRange</span></span>

<span data-ttu-id="2d97d-p101">Obtém um objeto que representa um intervalo deslocado do intervalo especificado. A dimensão do intervalo retornado corresponde a esse intervalo. Se o intervalo resultante é imposto para fora dos limites da grade da planilha, o sistema gera uma exceção.</span><span class="sxs-lookup"><span data-stu-id="2d97d-p101">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2d97d-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d97d-105">Prerequisites</span></span>
<span data-ttu-id="2d97d-106">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="2d97d-106">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="2d97d-107">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d97d-107">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="2d97d-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d97d-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/OffsetRange
GET /workbook/worksheets/{id|name}/range(<address>)/OffsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="2d97d-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d97d-109">Request headers</span></span>
| <span data-ttu-id="2d97d-110">Nome</span><span class="sxs-lookup"><span data-stu-id="2d97d-110">Name</span></span>       | <span data-ttu-id="2d97d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d97d-111">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2d97d-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d97d-112">Authorization</span></span>  | <span data-ttu-id="2d97d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d97d-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="2d97d-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d97d-115">Request body</span></span>
<span data-ttu-id="2d97d-116">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d97d-116">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2d97d-117">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2d97d-117">Parameter</span></span>    | <span data-ttu-id="2d97d-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d97d-118">Type</span></span>   |<span data-ttu-id="2d97d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d97d-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d97d-120">rowOffset</span><span class="sxs-lookup"><span data-stu-id="2d97d-120">rowOffset</span></span>|<span data-ttu-id="2d97d-121">number</span><span class="sxs-lookup"><span data-stu-id="2d97d-121">number</span></span>|<span data-ttu-id="2d97d-p103">O número de linhas (positivo, negativo ou 0) com base no qual o intervalo deve ser deslocado. Os valores positivos são deslocados para baixo e os negativos, para cima.</span><span class="sxs-lookup"><span data-stu-id="2d97d-p103">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="2d97d-124">columnOffset</span><span class="sxs-lookup"><span data-stu-id="2d97d-124">columnOffset</span></span>|<span data-ttu-id="2d97d-125">number</span><span class="sxs-lookup"><span data-stu-id="2d97d-125">number</span></span>|<span data-ttu-id="2d97d-p104">O número de colunas (positivo, negativo ou 0) com base no qual o intervalo deve ser deslocado. Os valores positivos são deslocados para a direita e os negativos, para a esquerda.</span><span class="sxs-lookup"><span data-stu-id="2d97d-p104">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="2d97d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d97d-128">Response</span></span>

<span data-ttu-id="2d97d-129">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d97d-129">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d97d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d97d-130">Example</span></span>
<span data-ttu-id="2d97d-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2d97d-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2d97d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d97d-132">Request</span></span>
<span data-ttu-id="2d97d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d97d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/OffsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": {
  },
  "columnOffset": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="2d97d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d97d-134">Response</span></span>
<span data-ttu-id="2d97d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d97d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: OffsetRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->