# <a name="list-chartpointscollection"></a><span data-ttu-id="9dd74-101">Listar ChartPointsCollection</span><span class="sxs-lookup"><span data-stu-id="9dd74-101">List ChartPointsCollection</span></span>

<span data-ttu-id="9dd74-102">Recupera uma lista de objetos chartpoint.</span><span class="sxs-lookup"><span data-stu-id="9dd74-102">Retrieve a list of chartpoint objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9dd74-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9dd74-103">Prerequisites</span></span>
<span data-ttu-id="9dd74-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="9dd74-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="9dd74-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9dd74-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="9dd74-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9dd74-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9dd74-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9dd74-107">Optional query parameters</span></span>
<span data-ttu-id="9dd74-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9dd74-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9dd74-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9dd74-109">Request headers</span></span>
| <span data-ttu-id="9dd74-110">Nome</span><span class="sxs-lookup"><span data-stu-id="9dd74-110">Name</span></span>      |<span data-ttu-id="9dd74-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9dd74-111">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9dd74-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="9dd74-112">Authorization</span></span>  | <span data-ttu-id="9dd74-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9dd74-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="9dd74-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9dd74-115">Request body</span></span>
<span data-ttu-id="9dd74-116">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9dd74-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9dd74-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="9dd74-117">Response</span></span>

<span data-ttu-id="9dd74-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ChartPoint](../resources/chartpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9dd74-118">If successful, this method returns a `200 OK` response code and collection of [ChartPoint](../resources/chartpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9dd74-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9dd74-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9dd74-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9dd74-120">Request</span></span>
<span data-ttu-id="9dd74-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9dd74-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartpointscollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
```
##### <a name="response"></a><span data-ttu-id="9dd74-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="9dd74-122">Response</span></span>
<span data-ttu-id="9dd74-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9dd74-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 57

{
  "value": [
    {
      "value": {
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List ChartPointsCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->