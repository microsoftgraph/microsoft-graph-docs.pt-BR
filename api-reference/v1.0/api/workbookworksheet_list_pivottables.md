# <a name="list-pivottables"></a><span data-ttu-id="451ff-101">Listar pivotTables</span><span class="sxs-lookup"><span data-stu-id="451ff-101">List pivotTables</span></span>

<span data-ttu-id="451ff-102">Recupere uma lista de objetos workbookpivottable.</span><span class="sxs-lookup"><span data-stu-id="451ff-102">Retrieve a list of workbookpivottable objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="451ff-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="451ff-103">Prerequisites</span></span>
<span data-ttu-id="451ff-104">Os seguintes **escopos** são necessários para executar esta API: _Files.Read, Files.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="451ff-104">The following **scopes** are required to execute this API: _Files.Read, Files.ReadWrite_</span></span>

## <a name="http-request"></a><span data-ttu-id="451ff-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="451ff-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="451ff-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="451ff-106">Optional query parameters</span></span>
<span data-ttu-id="451ff-107">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="451ff-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="451ff-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="451ff-108">Request headers</span></span>
| <span data-ttu-id="451ff-109">Nome</span><span class="sxs-lookup"><span data-stu-id="451ff-109">Name</span></span>      |<span data-ttu-id="451ff-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="451ff-110">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="451ff-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="451ff-111">Authorization</span></span>  | <span data-ttu-id="451ff-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="451ff-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="451ff-114">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="451ff-114">Workbook-Session-Id</span></span>  | <span data-ttu-id="451ff-p102">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="451ff-p102">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="451ff-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="451ff-117">Request body</span></span>
<span data-ttu-id="451ff-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="451ff-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="451ff-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="451ff-119">Response</span></span>

<span data-ttu-id="451ff-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [workbookPivotTable](../resources/workbookpivottable.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="451ff-120">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/workbookpivottable.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="451ff-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="451ff-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="451ff-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="451ff-122">Request</span></span>
<span data-ttu-id="451ff-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="451ff-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_pivottables"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables
```
##### <a name="response"></a><span data-ttu-id="451ff-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="451ff-124">Response</span></span>
<span data-ttu-id="451ff-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="451ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookPivotTable",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```
