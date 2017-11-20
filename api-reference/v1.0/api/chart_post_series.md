# <a name="create-chartseries"></a><span data-ttu-id="5882f-101">Criar ChartSeries</span><span class="sxs-lookup"><span data-stu-id="5882f-101">Create ChartSeries</span></span>

<span data-ttu-id="5882f-102">Use essa API para criar novas ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="5882f-102">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="5882f-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="5882f-103">Permissions</span></span>
<span data-ttu-id="5882f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5882f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5882f-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5882f-106">Permission type</span></span>      | <span data-ttu-id="5882f-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5882f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5882f-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5882f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5882f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5882f-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5882f-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5882f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5882f-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5882f-111">Not supported.</span></span>    |
|<span data-ttu-id="5882f-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5882f-112">Application</span></span> | <span data-ttu-id="5882f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5882f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5882f-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5882f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series

```
## <a name="request-headers"></a><span data-ttu-id="5882f-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5882f-115">Request headers</span></span>
| <span data-ttu-id="5882f-116">Nome</span><span class="sxs-lookup"><span data-stu-id="5882f-116">Name</span></span>       | <span data-ttu-id="5882f-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="5882f-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5882f-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="5882f-118">Authorization</span></span>  | <span data-ttu-id="5882f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5882f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5882f-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5882f-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="5882f-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5882f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5882f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5882f-124">Request body</span></span>
<span data-ttu-id="5882f-125">No corpo da solicitação, forneça uma representação JSON do objeto [ChartSeries](../resources/chartseries.md).</span><span class="sxs-lookup"><span data-stu-id="5882f-125">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5882f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5882f-126">Response</span></span>

<span data-ttu-id="5882f-127">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [ChartSeries](../resources/chartseries.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5882f-127">If successful, this method returns `201 Created` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5882f-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5882f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5882f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5882f-129">Request</span></span>
<span data-ttu-id="5882f-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5882f-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
<span data-ttu-id="5882f-131">No corpo da solicitação, forneça uma representação JSON do objeto [ChartSeries](../resources/chartseries.md).</span><span class="sxs-lookup"><span data-stu-id="5882f-131">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5882f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5882f-132">Response</span></span>
<span data-ttu-id="5882f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5882f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->