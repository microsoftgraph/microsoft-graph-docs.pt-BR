# <a name="tablerowcollection-add"></a><span data-ttu-id="36680-101">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="36680-101">TableRowCollection: add</span></span>

<span data-ttu-id="36680-102">Adiciona uma nova linha à tabela.</span><span class="sxs-lookup"><span data-stu-id="36680-102">Adds a new row to the table.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36680-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="36680-103">Prerequisites</span></span>
<span data-ttu-id="36680-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="36680-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="36680-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36680-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="36680-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36680-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="36680-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36680-107">Request headers</span></span>
| <span data-ttu-id="36680-108">Nome</span><span class="sxs-lookup"><span data-stu-id="36680-108">Name</span></span>       | <span data-ttu-id="36680-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="36680-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="36680-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="36680-110">Authorization</span></span>  | <span data-ttu-id="36680-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36680-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="36680-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36680-113">Request body</span></span>
<span data-ttu-id="36680-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36680-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="36680-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="36680-115">Parameter</span></span>    | <span data-ttu-id="36680-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="36680-116">Type</span></span>   |<span data-ttu-id="36680-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="36680-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36680-118">índice</span><span class="sxs-lookup"><span data-stu-id="36680-118">index</span></span>|<span data-ttu-id="36680-119">number</span><span class="sxs-lookup"><span data-stu-id="36680-119">number</span></span>|<span data-ttu-id="36680-p102">Opcional. Especifica a posição relativa da nova linha. Se for nulo, a adição ocorre no final. Todas as linhas abaixo da linha inserida serão deslocadas para baixo. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="36680-p102">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="36680-125">values</span><span class="sxs-lookup"><span data-stu-id="36680-125">values</span></span>|<span data-ttu-id="36680-126">(booliano, cadeia de caracteres ou número)</span><span class="sxs-lookup"><span data-stu-id="36680-126">(boolean or string or number)</span></span>|<span data-ttu-id="36680-p103">Opcional. Uma matriz bidimensional de valores não formatados da linha da tabela.</span><span class="sxs-lookup"><span data-stu-id="36680-p103">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="36680-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="36680-129">Response</span></span>

<span data-ttu-id="36680-130">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [TableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36680-130">If successful, this method returns `200, OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36680-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36680-131">Example</span></span>
<span data-ttu-id="36680-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="36680-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="36680-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36680-133">Request</span></span>
<span data-ttu-id="36680-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36680-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": null,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a><span data-ttu-id="36680-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="36680-135">Response</span></span>
<span data-ttu-id="36680-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36680-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
