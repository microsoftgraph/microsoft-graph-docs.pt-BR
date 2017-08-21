# <a name="create-tablecolumn"></a><span data-ttu-id="00054-101">Criar TableColumn</span><span class="sxs-lookup"><span data-stu-id="00054-101">Create TableColumn</span></span>

<span data-ttu-id="00054-102">Use essa API para criar uma nova TableColumn.</span><span class="sxs-lookup"><span data-stu-id="00054-102">Use this API to create a new TableColumn.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00054-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="00054-103">Prerequisites</span></span>
<span data-ttu-id="00054-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="00054-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="00054-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00054-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="00054-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00054-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="00054-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00054-107">Request headers</span></span>
| <span data-ttu-id="00054-108">Nome</span><span class="sxs-lookup"><span data-stu-id="00054-108">Name</span></span>       | <span data-ttu-id="00054-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="00054-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="00054-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="00054-110">Authorization</span></span>  | <span data-ttu-id="00054-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00054-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="00054-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00054-113">Request body</span></span>
<span data-ttu-id="00054-114">No corpo da solicitação, forneça uma representação JSON do objeto [TableColum](../resources/tablecolumn.md).</span><span class="sxs-lookup"><span data-stu-id="00054-114">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="00054-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="00054-115">Response</span></span>

<span data-ttu-id="00054-116">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [TableColumn](../resources/tablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00054-116">If successful, this method returns `201, Created` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00054-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00054-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00054-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00054-118">Request</span></span>
<span data-ttu-id="00054-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00054-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="00054-120">No corpo da solicitação, forneça uma representação JSON do objeto [TableColum](../resources/tablecolumn.md).</span><span class="sxs-lookup"><span data-stu-id="00054-120">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="00054-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="00054-121">Response</span></span>
<span data-ttu-id="00054-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00054-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->