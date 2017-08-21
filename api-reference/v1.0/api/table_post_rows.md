# <a name="create-tablerow"></a><span data-ttu-id="93966-101">Criar TableRow</span><span class="sxs-lookup"><span data-stu-id="93966-101">Create TableRow</span></span>

<span data-ttu-id="93966-102">Use essa API para criar uma nova TableRow.</span><span class="sxs-lookup"><span data-stu-id="93966-102">Use this API to create a new TableRow.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="93966-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="93966-103">Prerequisites</span></span>
<span data-ttu-id="93966-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="93966-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="93966-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93966-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="93966-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93966-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows

```
## <a name="request-headers"></a><span data-ttu-id="93966-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93966-107">Request headers</span></span>
| <span data-ttu-id="93966-108">Nome</span><span class="sxs-lookup"><span data-stu-id="93966-108">Name</span></span>       | <span data-ttu-id="93966-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="93966-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="93966-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="93966-110">Authorization</span></span>  | <span data-ttu-id="93966-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93966-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="93966-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93966-113">Request body</span></span>
<span data-ttu-id="93966-114">No corpo da solicitação, forneça uma representação JSON do objeto [TableRow](../resources/tablerow.md).</span><span class="sxs-lookup"><span data-stu-id="93966-114">In the request body, supply a JSON representation of [TableRow](../resources/tablerow.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="93966-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="93966-115">Response</span></span>

<span data-ttu-id="93966-116">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [TableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93966-116">If successful, this method returns `201, Created` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93966-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93966-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93966-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93966-118">Request</span></span>
<span data-ttu-id="93966-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93966-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablerow_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="93966-120">No corpo da solicitação, forneça uma representação JSON do objeto [TableRow](../resources/tablerow.md).</span><span class="sxs-lookup"><span data-stu-id="93966-120">In the request body, supply a JSON representation of [TableRow](../resources/tablerow.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="93966-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="93966-121">Response</span></span>
<span data-ttu-id="93966-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93966-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->