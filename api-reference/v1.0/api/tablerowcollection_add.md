# <a name="tablerowcollection-add"></a><span data-ttu-id="52dda-101">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="52dda-101">TableRowCollection: add</span></span>

<span data-ttu-id="52dda-102">Adiciona uma nova linha à tabela.</span><span class="sxs-lookup"><span data-stu-id="52dda-102">Adds a new row to the table.</span></span>

## <a name="error-handling"></a><span data-ttu-id="52dda-103">Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="52dda-103">Error Handling</span></span>

<span data-ttu-id="52dda-104">Essa solicitação poderá, ocasionalmente, receber uma mensagem de erro HTTP 504.</span><span class="sxs-lookup"><span data-stu-id="52dda-104">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="52dda-105">A resposta apropriada para esta mensagem de erro é repetir a solicitação.</span><span class="sxs-lookup"><span data-stu-id="52dda-105">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="52dda-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="52dda-106">Permissions</span></span>
<span data-ttu-id="52dda-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="52dda-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="52dda-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52dda-109">Permission type</span></span>      | <span data-ttu-id="52dda-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52dda-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52dda-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52dda-111">Delegated (work or school account)</span></span> | <span data-ttu-id="52dda-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52dda-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="52dda-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52dda-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52dda-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52dda-114">Not supported.</span></span>    |
|<span data-ttu-id="52dda-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52dda-115">Application</span></span> | <span data-ttu-id="52dda-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52dda-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52dda-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52dda-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="52dda-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52dda-118">Request headers</span></span>
| <span data-ttu-id="52dda-119">Nome</span><span class="sxs-lookup"><span data-stu-id="52dda-119">Name</span></span>       | <span data-ttu-id="52dda-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="52dda-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="52dda-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="52dda-121">Authorization</span></span>  | <span data-ttu-id="52dda-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52dda-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52dda-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="52dda-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="52dda-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="52dda-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52dda-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52dda-127">Request body</span></span>
<span data-ttu-id="52dda-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52dda-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="52dda-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="52dda-129">Parameter</span></span>    | <span data-ttu-id="52dda-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="52dda-130">Type</span></span>   |<span data-ttu-id="52dda-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="52dda-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52dda-132">índice</span><span class="sxs-lookup"><span data-stu-id="52dda-132">index</span></span>|<span data-ttu-id="52dda-133">number</span><span class="sxs-lookup"><span data-stu-id="52dda-133">number</span></span>|<span data-ttu-id="52dda-p105">Opcional. Especifica a posição relativa da nova linha. Se for nulo, a adição ocorre no final. Todas as linhas abaixo da linha inserida serão deslocadas para baixo. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="52dda-p105">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="52dda-139">values</span><span class="sxs-lookup"><span data-stu-id="52dda-139">values</span></span>|<span data-ttu-id="52dda-140">(booliano, cadeia de caracteres ou número)</span><span class="sxs-lookup"><span data-stu-id="52dda-140">(boolean or string or number)</span></span>|<span data-ttu-id="52dda-p106">Opcional. Uma matriz bidimensional de valores não formatados da linha da tabela.</span><span class="sxs-lookup"><span data-stu-id="52dda-p106">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="52dda-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="52dda-143">Response</span></span>

<span data-ttu-id="52dda-144">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [TableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52dda-144">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52dda-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52dda-145">Example</span></span>
<span data-ttu-id="52dda-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="52dda-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="52dda-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52dda-147">Request</span></span>
<span data-ttu-id="52dda-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52dda-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="52dda-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="52dda-149">Response</span></span>
<span data-ttu-id="52dda-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52dda-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
