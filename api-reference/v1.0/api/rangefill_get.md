# <a name="get-rangefill"></a><span data-ttu-id="71cd7-101">Obter RangeFill</span><span class="sxs-lookup"><span data-stu-id="71cd7-101">Get RangeFill</span></span>

<span data-ttu-id="71cd7-102">Recupere as propriedades e os relacionamentos do objeto rangefill.</span><span class="sxs-lookup"><span data-stu-id="71cd7-102">Retrieve the properties and relationships of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="71cd7-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="71cd7-103">Permissions</span></span>
<span data-ttu-id="71cd7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="71cd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71cd7-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71cd7-106">Permission type</span></span>      | <span data-ttu-id="71cd7-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71cd7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71cd7-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71cd7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="71cd7-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71cd7-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="71cd7-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71cd7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71cd7-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71cd7-111">Not supported.</span></span>    |
|<span data-ttu-id="71cd7-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71cd7-112">Application</span></span> | <span data-ttu-id="71cd7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71cd7-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71cd7-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71cd7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/format/fill
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/fill
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-query-parameters"></a><span data-ttu-id="71cd7-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="71cd7-115">Optional query parameters</span></span>
<span data-ttu-id="71cd7-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="71cd7-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71cd7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71cd7-117">Request headers</span></span>
| <span data-ttu-id="71cd7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="71cd7-118">Name</span></span>      |<span data-ttu-id="71cd7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="71cd7-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71cd7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="71cd7-120">Authorization</span></span>  | <span data-ttu-id="71cd7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71cd7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71cd7-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="71cd7-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="71cd7-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="71cd7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71cd7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71cd7-126">Request body</span></span>
<span data-ttu-id="71cd7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71cd7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71cd7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="71cd7-128">Response</span></span>

<span data-ttu-id="71cd7-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [RangeFill](../resources/rangefill.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71cd7-129">If successful, this method returns a `200 OK` response code and [RangeFill](../resources/rangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71cd7-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71cd7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71cd7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71cd7-131">Request</span></span>
<span data-ttu-id="71cd7-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71cd7-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rangefill"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/fill
```
##### <a name="response"></a><span data-ttu-id="71cd7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="71cd7-133">Response</span></span>
<span data-ttu-id="71cd7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71cd7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get RangeFill",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->