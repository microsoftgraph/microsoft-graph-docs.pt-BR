# <a name="tablerowcollection-add"></a><span data-ttu-id="d7d03-101">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="d7d03-101">TableRowCollection: add</span></span>

<span data-ttu-id="d7d03-102">Adiciona uma nova linha à tabela.</span><span class="sxs-lookup"><span data-stu-id="d7d03-102">Adds a new row to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7d03-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7d03-103">Permissions</span></span>
<span data-ttu-id="d7d03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d7d03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d7d03-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7d03-106">Permission type</span></span>      | <span data-ttu-id="d7d03-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d7d03-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7d03-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7d03-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d7d03-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7d03-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7d03-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7d03-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7d03-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7d03-111">Not supported.</span></span>    |
|<span data-ttu-id="d7d03-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7d03-112">Application</span></span> | <span data-ttu-id="d7d03-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7d03-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7d03-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7d03-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="d7d03-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7d03-115">Request headers</span></span>
| <span data-ttu-id="d7d03-116">Nome</span><span class="sxs-lookup"><span data-stu-id="d7d03-116">Name</span></span>       | <span data-ttu-id="d7d03-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7d03-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d7d03-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7d03-118">Authorization</span></span>  | <span data-ttu-id="d7d03-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7d03-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7d03-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d7d03-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="d7d03-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d7d03-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7d03-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7d03-124">Request body</span></span>
<span data-ttu-id="d7d03-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7d03-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d7d03-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d7d03-126">Parameter</span></span>    | <span data-ttu-id="d7d03-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7d03-127">Type</span></span>   |<span data-ttu-id="d7d03-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7d03-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7d03-129">index</span><span class="sxs-lookup"><span data-stu-id="d7d03-129">index</span></span>|<span data-ttu-id="d7d03-130">number</span><span class="sxs-lookup"><span data-stu-id="d7d03-130">number</span></span>|<span data-ttu-id="d7d03-p104">Opcional. Especifica a posição relativa da nova linha. Se for nulo, a adição ocorre no final. Todas as linhas abaixo da linha inserida serão deslocadas para baixo. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="d7d03-p104">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="d7d03-136">values</span><span class="sxs-lookup"><span data-stu-id="d7d03-136">values</span></span>|<span data-ttu-id="d7d03-137">(booliano, cadeia de caracteres ou número)</span><span class="sxs-lookup"><span data-stu-id="d7d03-137">(boolean or string or number)</span></span>|<span data-ttu-id="d7d03-p105">Opcional. Uma matriz bidimensional de valores não formatados da linha da tabela.</span><span class="sxs-lookup"><span data-stu-id="d7d03-p105">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="d7d03-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7d03-140">Response</span></span>

<span data-ttu-id="d7d03-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [TableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7d03-141">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7d03-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7d03-142">Example</span></span>
<span data-ttu-id="d7d03-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d7d03-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d7d03-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7d03-144">Request</span></span>
<span data-ttu-id="d7d03-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7d03-145">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d7d03-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7d03-146">Response</span></span>
<span data-ttu-id="d7d03-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7d03-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
