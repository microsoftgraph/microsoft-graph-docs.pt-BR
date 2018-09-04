# <a name="get-tablesort"></a><span data-ttu-id="aeb78-101">Obter TableSort</span><span class="sxs-lookup"><span data-stu-id="aeb78-101">Get TableSort</span></span>

<span data-ttu-id="aeb78-102">Recupere as propriedades e os relacionamentos do objeto tablesort.</span><span class="sxs-lookup"><span data-stu-id="aeb78-102">Retrieve the properties and relationships of tablesort object.</span></span>
## <a name="permissions"></a><span data-ttu-id="aeb78-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="aeb78-103">Permissions</span></span>
<span data-ttu-id="aeb78-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aeb78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aeb78-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aeb78-106">Permission type</span></span>      | <span data-ttu-id="aeb78-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aeb78-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aeb78-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aeb78-108">Delegated (work or school account)</span></span> | <span data-ttu-id="aeb78-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aeb78-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aeb78-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aeb78-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aeb78-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aeb78-111">Not supported.</span></span>    |
|<span data-ttu-id="aeb78-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aeb78-112">Application</span></span> | <span data-ttu-id="aeb78-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aeb78-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aeb78-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aeb78-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aeb78-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aeb78-115">Optional query parameters</span></span>
<span data-ttu-id="aeb78-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aeb78-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aeb78-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aeb78-117">Request headers</span></span>
| <span data-ttu-id="aeb78-118">Nome</span><span class="sxs-lookup"><span data-stu-id="aeb78-118">Name</span></span>      |<span data-ttu-id="aeb78-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="aeb78-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aeb78-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="aeb78-120">Authorization</span></span>  | <span data-ttu-id="aeb78-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aeb78-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aeb78-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="aeb78-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="aeb78-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="aeb78-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aeb78-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aeb78-126">Request body</span></span>
<span data-ttu-id="aeb78-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aeb78-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aeb78-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="aeb78-128">Response</span></span>

<span data-ttu-id="aeb78-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [WorkbookTableSort](../resources/tablesort.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aeb78-129">If successful, this method returns a `200 OK` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/tablesort.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aeb78-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aeb78-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aeb78-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aeb78-131">Request</span></span>
<span data-ttu-id="aeb78-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aeb78-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablesort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort
```
##### <a name="response"></a><span data-ttu-id="aeb78-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="aeb78-133">Response</span></span>
<span data-ttu-id="aeb78-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aeb78-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableSort"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "matchCase": true,
  "method": "method-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get TableSort",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->