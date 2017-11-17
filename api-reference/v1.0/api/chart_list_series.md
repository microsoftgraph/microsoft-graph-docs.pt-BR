# <a name="list-series"></a><span data-ttu-id="7cd0f-101">Listar séries</span><span class="sxs-lookup"><span data-stu-id="7cd0f-101">List series</span></span>

<span data-ttu-id="7cd0f-102">Recupere uma lista de objetos chartseries.</span><span class="sxs-lookup"><span data-stu-id="7cd0f-102">Retrieve a list of chartseries objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="7cd0f-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="7cd0f-103">Permissions</span></span>
<span data-ttu-id="7cd0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7cd0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7cd0f-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cd0f-106">Permission type</span></span>      | <span data-ttu-id="7cd0f-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7cd0f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cd0f-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cd0f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7cd0f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7cd0f-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7cd0f-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cd0f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cd0f-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cd0f-111">Not supported.</span></span>    |
|<span data-ttu-id="7cd0f-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7cd0f-112">Application</span></span> | <span data-ttu-id="7cd0f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cd0f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7cd0f-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cd0f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/series
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7cd0f-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7cd0f-115">Optional query parameters</span></span>
<span data-ttu-id="7cd0f-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7cd0f-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7cd0f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7cd0f-117">Request headers</span></span>
| <span data-ttu-id="7cd0f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7cd0f-118">Name</span></span>      |<span data-ttu-id="7cd0f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cd0f-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7cd0f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7cd0f-120">Authorization</span></span>  | <span data-ttu-id="7cd0f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cd0f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7cd0f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7cd0f-123">Request body</span></span>
<span data-ttu-id="7cd0f-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7cd0f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cd0f-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cd0f-125">Response</span></span>

<span data-ttu-id="7cd0f-126">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ChartSeries](../resources/chartseries.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7cd0f-126">If successful, this method returns a `200 OK` response code and collection of [ChartSeries](../resources/chartseries.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7cd0f-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7cd0f-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7cd0f-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cd0f-128">Request</span></span>
<span data-ttu-id="7cd0f-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7cd0f-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_series"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series
```
##### <a name="response"></a><span data-ttu-id="7cd0f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cd0f-130">Response</span></span>
<span data-ttu-id="7cd0f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7cd0f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 59

{
  "value": [
    {
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List series",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->