# <a name="list-rows"></a><span data-ttu-id="66921-101">Listar linhas</span><span class="sxs-lookup"><span data-stu-id="66921-101">List rows</span></span>

<span data-ttu-id="66921-102">Recupere uma lista de objetos tablerow.</span><span class="sxs-lookup"><span data-stu-id="66921-102">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="66921-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="66921-103">Permissions</span></span>
<span data-ttu-id="66921-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="66921-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="66921-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66921-106">Permission type</span></span>      | <span data-ttu-id="66921-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66921-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66921-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66921-108">Delegated (work or school account)</span></span> | <span data-ttu-id="66921-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66921-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="66921-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66921-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66921-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66921-111">Not supported.</span></span>    |
|<span data-ttu-id="66921-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66921-112">Application</span></span> | <span data-ttu-id="66921-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66921-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66921-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66921-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="66921-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="66921-115">Optional query parameters</span></span>
<span data-ttu-id="66921-116">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="66921-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>  <span data-ttu-id="66921-117">Para resultados confiáveis, use os parâmetros de consulta [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) e [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) para navegar pelos resultados.</span><span class="sxs-lookup"><span data-stu-id="66921-117">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="66921-118">Isso ajudará a evitar problemas de desempenho relacionados a grandes conjuntos de resultados.</span><span class="sxs-lookup"><span data-stu-id="66921-118">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66921-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66921-119">Request headers</span></span>
| <span data-ttu-id="66921-120">Nome</span><span class="sxs-lookup"><span data-stu-id="66921-120">Name</span></span>      |<span data-ttu-id="66921-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="66921-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="66921-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="66921-122">Authorization</span></span>  | <span data-ttu-id="66921-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66921-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66921-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="66921-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="66921-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="66921-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="66921-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66921-128">Request body</span></span>
<span data-ttu-id="66921-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="66921-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66921-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="66921-130">Response</span></span>

<span data-ttu-id="66921-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [WorkbookTableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66921-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableRow](../resources/tablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="66921-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66921-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66921-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66921-133">Request</span></span>
<span data-ttu-id="66921-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66921-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="66921-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="66921-135">Response</span></span>
<span data-ttu-id="66921-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66921-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 82

{
  "value": [
    {
      "index": 99,
      "values": "values-value"
    }
  ]
}
```
> <span data-ttu-id="66921-139">
  \*\*Observação:\*\* use os parâmetros de consulta [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) e [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) para navegar por um grande número de linhas.</span><span class="sxs-lookup"><span data-stu-id="66921-139">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="66921-140">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="66921-140">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5`


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rows",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->