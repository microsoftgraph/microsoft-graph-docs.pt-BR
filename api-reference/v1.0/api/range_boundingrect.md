# <a name="range-boundingrect"></a><span data-ttu-id="7339e-101">Range: BoundingRect</span><span class="sxs-lookup"><span data-stu-id="7339e-101">Range: BoundingRect</span></span>

<span data-ttu-id="7339e-p101">Obtém o menor objeto de intervalo que abrange os intervalos determinados. Por exemplo, GetBoundingRect de "B2:C5" e "D10:E15" é "B2:E16".</span><span class="sxs-lookup"><span data-stu-id="7339e-p101">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7339e-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7339e-104">Prerequisites</span></span>
<span data-ttu-id="7339e-105">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="7339e-105">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="7339e-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7339e-106">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="7339e-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7339e-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/BoundingRect
GET /workbook/worksheets/{id|name}/range(<address>)/BoundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/BoundingRect

```
## <a name="request-headers"></a><span data-ttu-id="7339e-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7339e-108">Request headers</span></span>
| <span data-ttu-id="7339e-109">Nome</span><span class="sxs-lookup"><span data-stu-id="7339e-109">Name</span></span>       | <span data-ttu-id="7339e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7339e-110">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7339e-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="7339e-111">Authorization</span></span>  | <span data-ttu-id="7339e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7339e-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="7339e-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7339e-114">Request body</span></span>
<span data-ttu-id="7339e-115">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7339e-115">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7339e-116">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7339e-116">Parameter</span></span>    | <span data-ttu-id="7339e-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="7339e-117">Type</span></span>   |<span data-ttu-id="7339e-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="7339e-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7339e-119">anotherRange</span><span class="sxs-lookup"><span data-stu-id="7339e-119">anotherRange</span></span>|<span data-ttu-id="7339e-120">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7339e-120">string</span></span>|<span data-ttu-id="7339e-121">O objeto de intervalo, endereço ou nome do intervalo.</span><span class="sxs-lookup"><span data-stu-id="7339e-121">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="7339e-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="7339e-122">Response</span></span>

<span data-ttu-id="7339e-123">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7339e-123">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7339e-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7339e-124">Example</span></span>
<span data-ttu-id="7339e-125">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7339e-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7339e-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7339e-126">Request</span></span>
<span data-ttu-id="7339e-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7339e-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/BoundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="7339e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7339e-128">Response</span></span>
<span data-ttu-id="7339e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7339e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->