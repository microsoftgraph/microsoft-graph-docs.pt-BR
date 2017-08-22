# <a name="tablerowcollection-itemat"></a><span data-ttu-id="e6abb-101">TableRowCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="e6abb-101">TableRowCollection: ItemAt</span></span>

<span data-ttu-id="e6abb-102">Obtém uma linha com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="e6abb-102">Gets a row based on its position in the collection.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e6abb-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e6abb-103">Prerequisites</span></span>
<span data-ttu-id="e6abb-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="e6abb-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="e6abb-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6abb-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="e6abb-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6abb-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/ItemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="e6abb-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6abb-107">Request headers</span></span>
| <span data-ttu-id="e6abb-108">Nome</span><span class="sxs-lookup"><span data-stu-id="e6abb-108">Name</span></span>       | <span data-ttu-id="e6abb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6abb-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e6abb-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6abb-110">Authorization</span></span>  | <span data-ttu-id="e6abb-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6abb-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e6abb-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6abb-113">Request body</span></span>
<span data-ttu-id="e6abb-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6abb-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e6abb-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e6abb-115">Parameter</span></span>    | <span data-ttu-id="e6abb-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6abb-116">Type</span></span>   |<span data-ttu-id="e6abb-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6abb-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6abb-118">índice</span><span class="sxs-lookup"><span data-stu-id="e6abb-118">index</span></span>|<span data-ttu-id="e6abb-119">number</span><span class="sxs-lookup"><span data-stu-id="e6abb-119">number</span></span>|<span data-ttu-id="e6abb-p102">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="e6abb-p102">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="e6abb-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6abb-122">Response</span></span>

<span data-ttu-id="e6abb-123">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [TableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6abb-123">If successful, this method returns `200, OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6abb-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6abb-124">Example</span></span>
<span data-ttu-id="e6abb-125">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e6abb-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e6abb-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6abb-126">Request</span></span>
<span data-ttu-id="e6abb-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6abb-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="e6abb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6abb-128">Response</span></span>
<span data-ttu-id="e6abb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6abb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "TableRowCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->