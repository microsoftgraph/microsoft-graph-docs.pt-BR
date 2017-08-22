# <a name="get-chartfont"></a><span data-ttu-id="0d0ee-101">Obter ChartFont</span><span class="sxs-lookup"><span data-stu-id="0d0ee-101">Get ChartFont</span></span>

<span data-ttu-id="0d0ee-102">Recupera as propriedades e os relacionamentos do objeto chartfont.</span><span class="sxs-lookup"><span data-stu-id="0d0ee-102">Retrieve the properties and relationships of chartfont object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0d0ee-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0d0ee-103">Prerequisites</span></span>
<span data-ttu-id="0d0ee-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="0d0ee-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="0d0ee-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d0ee-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="0d0ee-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d0ee-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
GET /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/font
GET /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/font
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0d0ee-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0d0ee-107">Optional query parameters</span></span>
<span data-ttu-id="0d0ee-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0d0ee-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d0ee-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d0ee-109">Request headers</span></span>
| <span data-ttu-id="0d0ee-110">Nome</span><span class="sxs-lookup"><span data-stu-id="0d0ee-110">Name</span></span>      |<span data-ttu-id="0d0ee-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d0ee-111">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0d0ee-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d0ee-112">Authorization</span></span>  | <span data-ttu-id="0d0ee-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d0ee-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0d0ee-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d0ee-115">Request body</span></span>
<span data-ttu-id="0d0ee-116">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d0ee-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d0ee-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d0ee-117">Response</span></span>

<span data-ttu-id="0d0ee-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartFont](../resources/chartfont.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d0ee-118">If successful, this method returns a `200 OK` response code and [ChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0d0ee-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d0ee-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d0ee-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d0ee-120">Request</span></span>
<span data-ttu-id="0d0ee-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d0ee-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartfont"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
```
##### <a name="response"></a><span data-ttu-id="0d0ee-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d0ee-122">Response</span></span>
<span data-ttu-id="0d0ee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d0ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartFont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->