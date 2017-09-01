# <a name="list-tablecollection"></a><span data-ttu-id="0a4f7-101">Listar TableCollection</span><span class="sxs-lookup"><span data-stu-id="0a4f7-101">List TableCollection</span></span>

<span data-ttu-id="0a4f7-102">Recupere uma lista de objetos de tabela.</span><span class="sxs-lookup"><span data-stu-id="0a4f7-102">Retrieve a list of table objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="0a4f7-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="0a4f7-103">Permissions</span></span>
<span data-ttu-id="0a4f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0a4f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0a4f7-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a4f7-106">Permission type</span></span>      | <span data-ttu-id="0a4f7-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a4f7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a4f7-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a4f7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0a4f7-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a4f7-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0a4f7-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a4f7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a4f7-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a4f7-111">Not supported.</span></span>    |
|<span data-ttu-id="0a4f7-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a4f7-112">Application</span></span> | <span data-ttu-id="0a4f7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a4f7-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a4f7-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a4f7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables
GET /workbook/worksheets/{id|name}/tables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0a4f7-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0a4f7-115">Optional query parameters</span></span>
<span data-ttu-id="0a4f7-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0a4f7-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a4f7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a4f7-117">Request headers</span></span>
| <span data-ttu-id="0a4f7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0a4f7-118">Name</span></span>      |<span data-ttu-id="0a4f7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a4f7-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0a4f7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a4f7-120">Authorization</span></span>  | <span data-ttu-id="0a4f7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a4f7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a4f7-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a4f7-123">Request body</span></span>
<span data-ttu-id="0a4f7-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0a4f7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a4f7-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a4f7-125">Response</span></span>

<span data-ttu-id="0a4f7-126">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Table](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a4f7-126">If successful, this method returns a `200 OK` response code and collection of [Table](../resources/table.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0a4f7-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a4f7-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a4f7-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a4f7-128">Request</span></span>
<span data-ttu-id="0a4f7-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a4f7-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables
```
##### <a name="response"></a><span data-ttu-id="0a4f7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a4f7-130">Response</span></span>
<span data-ttu-id="0a4f7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a4f7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "id": "99",
      "name": "name-value",
      "showHeaders": true,
      "showTotals": true,
      "style": "style-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TableCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
