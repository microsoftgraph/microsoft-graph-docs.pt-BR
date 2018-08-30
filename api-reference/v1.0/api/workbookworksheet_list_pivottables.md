# <a name="list-pivottables"></a><span data-ttu-id="7541b-101">Listar pivotTables</span><span class="sxs-lookup"><span data-stu-id="7541b-101">List pivotTables</span></span>

<span data-ttu-id="7541b-102">Recupere uma lista de objetos workbookpivottable.</span><span class="sxs-lookup"><span data-stu-id="7541b-102">Retrieve a list of workbookpivottable objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7541b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="7541b-103">Permissions</span></span>
<span data-ttu-id="7541b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7541b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="7541b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7541b-106">Permission type</span></span>      | <span data-ttu-id="7541b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7541b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7541b-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7541b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7541b-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7541b-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7541b-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7541b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7541b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7541b-111">Not supported.</span></span>    |
|<span data-ttu-id="7541b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7541b-112">Application</span></span> | <span data-ttu-id="7541b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7541b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7541b-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7541b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7541b-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7541b-115">Optional query parameters</span></span>
<span data-ttu-id="7541b-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7541b-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7541b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7541b-117">Request headers</span></span>
| <span data-ttu-id="7541b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7541b-118">Name</span></span>      |<span data-ttu-id="7541b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7541b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7541b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7541b-120">Authorization</span></span>  | <span data-ttu-id="7541b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7541b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7541b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7541b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7541b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7541b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7541b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7541b-126">Request body</span></span>
<span data-ttu-id="7541b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7541b-127">Do not supply a request body for this method.</span></span>
### <a name="response"></a><span data-ttu-id="7541b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7541b-128">Response</span></span>
<span data-ttu-id="7541b-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [workbookPivotTable](../resources/workbookpivottable.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7541b-129">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/workbookpivottable.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7541b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7541b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7541b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7541b-131">Request</span></span>
<span data-ttu-id="7541b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7541b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_pivottables"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables
```
##### <a name="response"></a><span data-ttu-id="7541b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7541b-133">Response</span></span>
<span data-ttu-id="7541b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7541b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
