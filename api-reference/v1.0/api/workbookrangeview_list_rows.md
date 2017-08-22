# <a name="list-rangeview-rows"></a><span data-ttu-id="db17e-101">Linhas da lista rangeView</span><span class="sxs-lookup"><span data-stu-id="db17e-101">List rangeView rows</span></span>

<span data-ttu-id="db17e-102">Recupere uma lista de objetos da exibição de intervalo.</span><span class="sxs-lookup"><span data-stu-id="db17e-102">Retrieve a list of range view objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db17e-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="db17e-103">Prerequisites</span></span>
<span data-ttu-id="db17e-104">Os seguintes **escopos** são necessários para executar esta API: _Files.Read, Files.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="db17e-104">The following **scopes** are required to execute this API: _Files.Read, Files.ReadWrite_</span></span>
## <a name="http-request"></a><span data-ttu-id="db17e-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db17e-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/rows

```
## <a name="optional-query-parameters"></a><span data-ttu-id="db17e-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="db17e-106">Optional query parameters</span></span>
<span data-ttu-id="db17e-107">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="db17e-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db17e-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db17e-108">Request headers</span></span>
| <span data-ttu-id="db17e-109">Nome</span><span class="sxs-lookup"><span data-stu-id="db17e-109">Name</span></span>      |<span data-ttu-id="db17e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="db17e-110">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="db17e-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="db17e-111">Authorization</span></span>  | <span data-ttu-id="db17e-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db17e-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db17e-114">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="db17e-114">Workbook-Session-Id</span></span>  | <span data-ttu-id="db17e-p102">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="db17e-p102">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db17e-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db17e-117">Request body</span></span>
<span data-ttu-id="db17e-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="db17e-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db17e-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="db17e-119">Response</span></span>

<span data-ttu-id="db17e-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db17e-120">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/workbookrangeview.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db17e-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db17e-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db17e-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db17e-122">Request</span></span>
<span data-ttu-id="db17e-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db17e-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/rows 
```
##### <a name="response"></a><span data-ttu-id="db17e-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="db17e-124">Response</span></span>
<span data-ttu-id="db17e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db17e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 247

{
  "value": [
    {
      "cellAddresses": "cellAddresses-value",
      "columnCount": 99,
      "formulas": "formulas-value",
      "formulasLocal": "formulasLocal-value",
      "formulasR1C1": "formulasR1C1-value",
      "index": 99
    }
  ]
}
```
