# <a name="create-tablerow"></a><span data-ttu-id="cbf5d-101">Criar TableRow</span><span class="sxs-lookup"><span data-stu-id="cbf5d-101">Create TableRow</span></span>

<span data-ttu-id="cbf5d-102">Adiciona linhas ao final da tabela.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-102">Adds a row to the end of the table.</span></span> <span data-ttu-id="cbf5d-103">Observe que a API pode aceitar dados de várias linhas usando essa API.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-103">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="cbf5d-104">Adicionar uma linha por vez pode levar à degradação do desempenho.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-104">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="cbf5d-105">A abordagem recomendada seria agrupar as linhas em uma única chamada em vez de fazer a inserção de uma linha por vez.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-105">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="cbf5d-106">Para obter melhores resultados, colete as linhas a serem inseridas no lado do aplicativo e realize uma única operação de adição de linha.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-106">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="cbf5d-107">Teste números de linhas para determinar o número ideal para usar em única chamada de API.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-107">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="cbf5d-108">Manipulação de erro</span><span class="sxs-lookup"><span data-stu-id="cbf5d-108">Error Handling</span></span>

<span data-ttu-id="cbf5d-109">Essa solicitação poderá, ocasionalmente, receber uma mensagem de erro HTTP 504.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-109">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="cbf5d-110">A resposta apropriada para esta mensagem de erro é repetir a solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-110">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbf5d-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="cbf5d-111">Permissions</span></span>
<span data-ttu-id="cbf5d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cbf5d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cbf5d-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbf5d-114">Permission type</span></span>      | <span data-ttu-id="cbf5d-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbf5d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbf5d-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbf5d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="cbf5d-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbf5d-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cbf5d-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbf5d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbf5d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-119">Not supported.</span></span>    |
|<span data-ttu-id="cbf5d-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbf5d-120">Application</span></span> | <span data-ttu-id="cbf5d-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbf5d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbf5d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="cbf5d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbf5d-123">Request headers</span></span>
| <span data-ttu-id="cbf5d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="cbf5d-124">Name</span></span>       | <span data-ttu-id="cbf5d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbf5d-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cbf5d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbf5d-126">Authorization</span></span>  | <span data-ttu-id="cbf5d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cbf5d-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cbf5d-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="cbf5d-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbf5d-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbf5d-132">Request body</span></span>
<span data-ttu-id="cbf5d-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cbf5d-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cbf5d-134">Parameter</span></span>    | <span data-ttu-id="cbf5d-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbf5d-135">Type</span></span>   |<span data-ttu-id="cbf5d-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbf5d-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbf5d-137">índice</span><span class="sxs-lookup"><span data-stu-id="cbf5d-137">index</span></span>|<span data-ttu-id="cbf5d-138">número</span><span class="sxs-lookup"><span data-stu-id="cbf5d-138">number</span></span>|<span data-ttu-id="cbf5d-p106">Opcional. Especifica a posição relativa da nova linha. Se for nulo, a adição ocorre no final. Todas as linhas abaixo da linha inserida serão deslocadas para baixo. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-p106">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="cbf5d-144">values</span><span class="sxs-lookup"><span data-stu-id="cbf5d-144">values</span></span>|<span data-ttu-id="cbf5d-145">Json</span><span class="sxs-lookup"><span data-stu-id="cbf5d-145">Json</span></span>|<span data-ttu-id="cbf5d-146">Uma matriz bidimensional dos valores não formatados das linhas da tabela (booleano ou sequência de caracteres ou número).</span><span class="sxs-lookup"><span data-stu-id="cbf5d-146">A 2-dimensional array of unformatted values of the table rows (boolean or string or number).</span></span>|

## <a name="response"></a><span data-ttu-id="cbf5d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbf5d-147">Response</span></span>

<span data-ttu-id="cbf5d-148">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [TableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-148">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbf5d-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbf5d-149">Example</span></span>
<span data-ttu-id="cbf5d-150">Neste exemplo, duas linhas de dados são inseridas no fim da tabela.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-150">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="cbf5d-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbf5d-151">Request</span></span>
<span data-ttu-id="cbf5d-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```
##### <a name="response"></a><span data-ttu-id="cbf5d-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbf5d-153">Response</span></span>
<span data-ttu-id="cbf5d-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbf5d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
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
  "suppressions": [
    "Error: /api-reference/v1.0/api/table_post_rows.md/tablerowcollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not.",
    "Warning: /api-reference/v1.0/api/table_post_rows.md/tablerowcollection_add/values:
      Inconsistent types between parameter (Collection) and table (None)"
  ],
  "tocPath": ""
}-->
