# <a name="get-charttitle"></a><span data-ttu-id="1aef6-101">Obter ChartTitle</span><span class="sxs-lookup"><span data-stu-id="1aef6-101">Get ChartTitle</span></span>

<span data-ttu-id="1aef6-102">Recupera as propriedades e os relacionamentos do objeto charttitle.</span><span class="sxs-lookup"><span data-stu-id="1aef6-102">Retrieve the properties and relationships of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1aef6-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="1aef6-103">Permissions</span></span>
<span data-ttu-id="1aef6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1aef6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1aef6-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1aef6-106">Permission type</span></span>      | <span data-ttu-id="1aef6-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1aef6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1aef6-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1aef6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1aef6-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1aef6-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1aef6-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1aef6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1aef6-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1aef6-111">Not supported.</span></span>    |
|<span data-ttu-id="1aef6-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1aef6-112">Application</span></span> | <span data-ttu-id="1aef6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1aef6-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1aef6-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1aef6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1aef6-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1aef6-115">Optional query parameters</span></span>
<span data-ttu-id="1aef6-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1aef6-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1aef6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1aef6-117">Request headers</span></span>
| <span data-ttu-id="1aef6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1aef6-118">Name</span></span>      |<span data-ttu-id="1aef6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1aef6-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1aef6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="1aef6-120">Authorization</span></span>  | <span data-ttu-id="1aef6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1aef6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1aef6-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1aef6-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="1aef6-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1aef6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1aef6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1aef6-126">Request body</span></span>
<span data-ttu-id="1aef6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1aef6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1aef6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1aef6-128">Response</span></span>

<span data-ttu-id="1aef6-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [WorkbookChartTitle](../resources/charttitle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1aef6-129">If successful, this method returns a `200 OK` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1aef6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1aef6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1aef6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1aef6-131">Request</span></span>
<span data-ttu-id="1aef6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1aef6-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_charttitle"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
```
##### <a name="response"></a><span data-ttu-id="1aef6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1aef6-133">Response</span></span>
<span data-ttu-id="1aef6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1aef6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->