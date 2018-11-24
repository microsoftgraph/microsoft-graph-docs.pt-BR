# <a name="list-names"></a><span data-ttu-id="2723d-101">Listar nomes</span><span class="sxs-lookup"><span data-stu-id="2723d-101">List names</span></span>

<span data-ttu-id="2723d-102">Recupere uma lista de itens nomeados associados à planilha.</span><span class="sxs-lookup"><span data-stu-id="2723d-102">Retrieve a list of named item associated with the worksheet.</span></span> 
## <a name="permissions"></a><span data-ttu-id="2723d-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="2723d-103">Permissions</span></span>
<span data-ttu-id="2723d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2723d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2723d-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2723d-106">Permission type</span></span>      | <span data-ttu-id="2723d-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2723d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2723d-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2723d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2723d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2723d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2723d-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2723d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2723d-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2723d-111">Not supported.</span></span>    |
|<span data-ttu-id="2723d-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2723d-112">Application</span></span> | <span data-ttu-id="2723d-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="2723d-113">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2723d-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2723d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets({id|name})/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2723d-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2723d-115">Optional query parameters</span></span>
<span data-ttu-id="2723d-116">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2723d-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2723d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2723d-117">Request headers</span></span>
| <span data-ttu-id="2723d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2723d-118">Name</span></span>      |<span data-ttu-id="2723d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2723d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2723d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2723d-120">Authorization</span></span>  | <span data-ttu-id="2723d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2723d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2723d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2723d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2723d-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2723d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2723d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2723d-126">Request body</span></span>
<span data-ttu-id="2723d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2723d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2723d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2723d-128">Response</span></span>

<span data-ttu-id="2723d-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [WorkbookNamedItem](../resources/nameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2723d-129">If successful, this method returns a `200 OK` response code and collection of [WorkbookNamedItem](../resources/nameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2723d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2723d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2723d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2723d-131">Request</span></span>
<span data-ttu-id="2723d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2723d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tables"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/names
```
##### <a name="response"></a><span data-ttu-id="2723d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2723d-133">Response</span></span>
<span data-ttu-id="2723d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2723d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "name": "myrange",
      "scope": "worksheet"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tables",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
