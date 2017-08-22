# <a name="range-intersection"></a><span data-ttu-id="6fca7-101">Range: Intersection</span><span class="sxs-lookup"><span data-stu-id="6fca7-101">Range: Intersection</span></span>

<span data-ttu-id="6fca7-102">Obtém o objeto de intervalo que representa a interseção retangular dos intervalos determinados.</span><span class="sxs-lookup"><span data-stu-id="6fca7-102">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6fca7-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6fca7-103">Prerequisites</span></span>
<span data-ttu-id="6fca7-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="6fca7-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="6fca7-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6fca7-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="6fca7-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fca7-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Intersection
GET /workbook/worksheets/{id|name}/range(<address>)/Intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/Intersection

```
## <a name="request-headers"></a><span data-ttu-id="6fca7-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fca7-107">Request headers</span></span>
| <span data-ttu-id="6fca7-108">Nome</span><span class="sxs-lookup"><span data-stu-id="6fca7-108">Name</span></span>       | <span data-ttu-id="6fca7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fca7-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6fca7-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fca7-110">Authorization</span></span>  | <span data-ttu-id="6fca7-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fca7-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="6fca7-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fca7-113">Request body</span></span>
<span data-ttu-id="6fca7-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fca7-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6fca7-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6fca7-115">Parameter</span></span>    | <span data-ttu-id="6fca7-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fca7-116">Type</span></span>   |<span data-ttu-id="6fca7-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fca7-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fca7-118">anotherRange</span><span class="sxs-lookup"><span data-stu-id="6fca7-118">anotherRange</span></span>|<span data-ttu-id="6fca7-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6fca7-119">string</span></span>|<span data-ttu-id="6fca7-120">O objeto de intervalo ou o endereço do intervalo que será usado para determinar a interseção de intervalos.</span><span class="sxs-lookup"><span data-stu-id="6fca7-120">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="6fca7-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fca7-121">Response</span></span>

<span data-ttu-id="6fca7-122">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fca7-122">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fca7-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fca7-123">Example</span></span>
<span data-ttu-id="6fca7-124">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6fca7-124">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6fca7-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fca7-125">Request</span></span>
<span data-ttu-id="6fca7-126">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fca7-126">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/Intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="6fca7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fca7-127">Response</span></span>
<span data-ttu-id="6fca7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6fca7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->