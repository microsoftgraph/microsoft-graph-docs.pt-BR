# <a name="create-chart"></a><span data-ttu-id="e2537-101">Criar gráfico</span><span class="sxs-lookup"><span data-stu-id="e2537-101">Create Chart</span></span>

<span data-ttu-id="e2537-102">Use esta API para criar um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="e2537-102">Use this API to create a new Chart.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e2537-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e2537-103">Prerequisites</span></span>
<span data-ttu-id="e2537-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="e2537-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="e2537-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2537-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="e2537-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2537-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="e2537-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2537-107">Request headers</span></span>
| <span data-ttu-id="e2537-108">Nome</span><span class="sxs-lookup"><span data-stu-id="e2537-108">Name</span></span>       | <span data-ttu-id="e2537-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2537-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e2537-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2537-110">Authorization</span></span>  | <span data-ttu-id="e2537-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2537-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e2537-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2537-113">Request body</span></span>
<span data-ttu-id="e2537-114">No corpo da solicitação, forneça uma representação JSON do objeto [Chart](../resources/chart.md).</span><span class="sxs-lookup"><span data-stu-id="e2537-114">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e2537-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2537-115">Response</span></span>

<span data-ttu-id="e2537-116">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [Chart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2537-116">If successful, this method returns `201, Created` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2537-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2537-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2537-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2537-118">Request</span></span>
<span data-ttu-id="e2537-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2537-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
<span data-ttu-id="e2537-120">No corpo da solicitação, forneça uma representação JSON do objeto [Chart](../resources/chart.md).</span><span class="sxs-lookup"><span data-stu-id="e2537-120">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e2537-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2537-121">Response</span></span>
<span data-ttu-id="e2537-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2537-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->