# <a name="get-formatprotection"></a><span data-ttu-id="54b0a-101">Obter FormatProtection</span><span class="sxs-lookup"><span data-stu-id="54b0a-101">Get FormatProtection</span></span>

<span data-ttu-id="54b0a-102">Recupere as propriedades e os relacionamentos do objeto formatprotection.</span><span class="sxs-lookup"><span data-stu-id="54b0a-102">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="54b0a-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="54b0a-103">Permissions</span></span>
<span data-ttu-id="54b0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="54b0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="54b0a-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54b0a-106">Permission type</span></span>      | <span data-ttu-id="54b0a-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54b0a-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="54b0a-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54b0a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="54b0a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54b0a-109">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="54b0a-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54b0a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54b0a-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54b0a-111">Not supported.</span></span>    | 
|<span data-ttu-id="54b0a-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54b0a-112">Application</span></span> | <span data-ttu-id="54b0a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54b0a-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="54b0a-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54b0a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/protection
GET /workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="54b0a-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="54b0a-115">Optional query parameters</span></span>
<span data-ttu-id="54b0a-116">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="54b0a-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54b0a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54b0a-117">Request headers</span></span>
| <span data-ttu-id="54b0a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="54b0a-118">Name</span></span>      |<span data-ttu-id="54b0a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="54b0a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="54b0a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="54b0a-120">Authorization</span></span>  | <span data-ttu-id="54b0a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54b0a-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="54b0a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54b0a-123">Request body</span></span>
<span data-ttu-id="54b0a-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="54b0a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54b0a-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="54b0a-125">Response</span></span>

<span data-ttu-id="54b0a-126">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [FormatProtection](../resources/formatprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54b0a-126">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="54b0a-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54b0a-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54b0a-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54b0a-128">Request</span></span>
<span data-ttu-id="54b0a-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54b0a-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/protection
```
##### <a name="response"></a><span data-ttu-id="54b0a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="54b0a-130">Response</span></span>
<span data-ttu-id="54b0a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54b0a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookFormatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get FormatProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->