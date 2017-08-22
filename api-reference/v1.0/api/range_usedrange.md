# <a name="range-usedrange"></a><span data-ttu-id="be317-101">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="be317-101">Range: UsedRange</span></span>

<span data-ttu-id="be317-102">Retorna o intervalo usado do objeto range determinado.</span><span class="sxs-lookup"><span data-stu-id="be317-102">Returns the used range of the given range object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be317-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="be317-103">Prerequisites</span></span>
<span data-ttu-id="be317-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="be317-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="be317-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be317-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="be317-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be317-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/UsedRange
GET /workbook/worksheets/{id|name}/range(<address>)/UsedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="be317-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be317-107">Request headers</span></span>
| <span data-ttu-id="be317-108">Nome</span><span class="sxs-lookup"><span data-stu-id="be317-108">Name</span></span>       | <span data-ttu-id="be317-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="be317-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="be317-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="be317-110">Authorization</span></span>  | <span data-ttu-id="be317-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be317-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="be317-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be317-113">Request body</span></span>
<span data-ttu-id="be317-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be317-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="be317-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="be317-115">Parameter</span></span>    | <span data-ttu-id="be317-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="be317-116">Type</span></span>   |<span data-ttu-id="be317-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="be317-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be317-118">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="be317-118">valuesOnly</span></span>|<span data-ttu-id="be317-119">booliano</span><span class="sxs-lookup"><span data-stu-id="be317-119">boolean</span></span>|<span data-ttu-id="be317-p102">Opcional. Considera apenas as células com valores como células usadas.</span><span class="sxs-lookup"><span data-stu-id="be317-p102">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="be317-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="be317-122">Response</span></span>

<span data-ttu-id="be317-123">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be317-123">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be317-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be317-124">Example</span></span>
<span data-ttu-id="be317-125">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="be317-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="be317-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be317-126">Request</span></span>
<span data-ttu-id="be317-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be317-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/UsedRange
Content-type: application/json
Content-length: 24

{
  "valuesOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="be317-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="be317-128">Response</span></span>
<span data-ttu-id="be317-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be317-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->