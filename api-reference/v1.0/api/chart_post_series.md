# <a name="create-chartseries"></a><span data-ttu-id="486ce-101">Criar ChartSeries</span><span class="sxs-lookup"><span data-stu-id="486ce-101">Create ChartSeries</span></span>

<span data-ttu-id="486ce-102">Use essa API para criar novas ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="486ce-102">Use this API to create a new ChartSeries.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="486ce-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="486ce-103">Prerequisites</span></span>
<span data-ttu-id="486ce-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="486ce-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="486ce-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="486ce-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="486ce-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="486ce-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series

```
## <a name="request-headers"></a><span data-ttu-id="486ce-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="486ce-107">Request headers</span></span>
| <span data-ttu-id="486ce-108">Nome</span><span class="sxs-lookup"><span data-stu-id="486ce-108">Name</span></span>       | <span data-ttu-id="486ce-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="486ce-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="486ce-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="486ce-110">Authorization</span></span>  | <span data-ttu-id="486ce-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="486ce-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="486ce-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="486ce-113">Request body</span></span>
<span data-ttu-id="486ce-114">No corpo da solicitação, forneça uma representação JSON do objeto [ChartSeries](../resources/chartseries.md).</span><span class="sxs-lookup"><span data-stu-id="486ce-114">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="486ce-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="486ce-115">Response</span></span>

<span data-ttu-id="486ce-116">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [ChartSeries](../resources/chartseries.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="486ce-116">If successful, this method returns `201, Created` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="486ce-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="486ce-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="486ce-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="486ce-118">Request</span></span>
<span data-ttu-id="486ce-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="486ce-119">Here is an example of the request.</span></span>
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
<span data-ttu-id="486ce-120">No corpo da solicitação, forneça uma representação JSON do objeto [ChartSeries](../resources/chartseries.md).</span><span class="sxs-lookup"><span data-stu-id="486ce-120">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="486ce-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="486ce-121">Response</span></span>
<span data-ttu-id="486ce-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="486ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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