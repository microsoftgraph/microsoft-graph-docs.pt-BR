# <a name="tablecolumncollection-add"></a><span data-ttu-id="d4986-101">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="d4986-101">TableColumnCollection: add</span></span>

<span data-ttu-id="d4986-102">Adiciona uma nova coluna à tabela.</span><span class="sxs-lookup"><span data-stu-id="d4986-102">Adds a new column to the table.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4986-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4986-103">Prerequisites</span></span>
<span data-ttu-id="d4986-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="d4986-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="d4986-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4986-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="d4986-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4986-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="d4986-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4986-107">Request headers</span></span>
| <span data-ttu-id="d4986-108">Nome</span><span class="sxs-lookup"><span data-stu-id="d4986-108">Name</span></span>       | <span data-ttu-id="d4986-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4986-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d4986-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4986-110">Authorization</span></span>  | <span data-ttu-id="d4986-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4986-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d4986-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4986-113">Request body</span></span>
<span data-ttu-id="d4986-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4986-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d4986-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d4986-115">Parameter</span></span>    | <span data-ttu-id="d4986-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4986-116">Type</span></span>   |<span data-ttu-id="d4986-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4986-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4986-118">índice</span><span class="sxs-lookup"><span data-stu-id="d4986-118">index</span></span>|<span data-ttu-id="d4986-119">number</span><span class="sxs-lookup"><span data-stu-id="d4986-119">number</span></span>|<span data-ttu-id="d4986-p102">Especifica a posição relativa da nova coluna. A coluna anterior nessa posição é deslocada para a direita. O valor do índice deve ser igual ou menor que o valor do índice da última coluna, portanto não pode ser usado para acrescentar uma coluna ao final da tabela. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="d4986-p102">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="d4986-124">values</span><span class="sxs-lookup"><span data-stu-id="d4986-124">values</span></span>|<span data-ttu-id="d4986-125">(booliano, cadeia de caracteres ou número)</span><span class="sxs-lookup"><span data-stu-id="d4986-125">(boolean or string or number)</span></span>|<span data-ttu-id="d4986-p103">Opcional. Uma matriz bidimensional de valores não formatados da coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="d4986-p103">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="d4986-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4986-128">Response</span></span>

<span data-ttu-id="d4986-129">Se bem-sucedido, este método retorna um código de resposta `200, OK` e um objeto [TableColumn](../resources/tablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4986-129">If successful, this method returns `200, OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4986-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4986-130">Example</span></span>
<span data-ttu-id="d4986-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d4986-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d4986-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4986-132">Request</span></span>
<span data-ttu-id="d4986-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4986-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": {
  },
  "values": [
    {
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="d4986-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4986-134">Response</span></span>
<span data-ttu-id="d4986-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4986-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->