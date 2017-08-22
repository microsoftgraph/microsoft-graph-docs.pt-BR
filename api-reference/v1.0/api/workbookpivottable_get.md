# <a name="get-workbookpivottable"></a><span data-ttu-id="60ad4-101">Obter workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="60ad4-101">Get workbookPivotTable</span></span>

<span data-ttu-id="60ad4-102">Recupere as propriedades e relações do objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="60ad4-102">Retrieve the properties and relationships of workbookPivotTable object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60ad4-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60ad4-103">Prerequisites</span></span>
<span data-ttu-id="60ad4-104">Os seguintes **escopos** são necessários para executar esta API: _Files.Read, Files.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="60ad4-104">The following **scopes** are required to execute this API: _Files.Read, Files.ReadWrite_</span></span>

## <a name="http-request"></a><span data-ttu-id="60ad4-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60ad4-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="60ad4-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="60ad4-106">Optional query parameters</span></span>
<span data-ttu-id="60ad4-107">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="60ad4-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60ad4-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60ad4-108">Request headers</span></span>
| <span data-ttu-id="60ad4-109">Nome</span><span class="sxs-lookup"><span data-stu-id="60ad4-109">Name</span></span>      |<span data-ttu-id="60ad4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="60ad4-110">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="60ad4-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="60ad4-111">Authorization</span></span>  | <span data-ttu-id="60ad4-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60ad4-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="60ad4-114">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="60ad4-114">Workbook-Session-Id</span></span>  | <span data-ttu-id="60ad4-p102">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="60ad4-p102">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60ad4-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60ad4-117">Request body</span></span>
<span data-ttu-id="60ad4-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60ad4-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60ad4-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="60ad4-119">Response</span></span>

<span data-ttu-id="60ad4-120">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [workbookPivotTable](../resources/workbookpivottable.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60ad4-120">If successful, this method returns a `200 OK` response code and [workbookPivotTable](../resources/workbookpivottable.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="60ad4-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60ad4-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60ad4-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60ad4-122">Request</span></span>
<span data-ttu-id="60ad4-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60ad4-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookpivottable"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
##### <a name="response"></a><span data-ttu-id="60ad4-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="60ad4-124">Response</span></span>
<span data-ttu-id="60ad4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60ad4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookPivotTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```
