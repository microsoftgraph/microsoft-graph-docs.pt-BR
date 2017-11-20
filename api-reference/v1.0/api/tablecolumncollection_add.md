# <a name="tablecolumncollection-add"></a><span data-ttu-id="44154-101">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="44154-101">TableColumnCollection: add</span></span>

<span data-ttu-id="44154-102">Adiciona uma nova coluna à tabela.</span><span class="sxs-lookup"><span data-stu-id="44154-102">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="44154-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="44154-103">Permissions</span></span>
<span data-ttu-id="44154-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="44154-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="44154-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44154-106">Permission type</span></span>      | <span data-ttu-id="44154-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="44154-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44154-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44154-108">Delegated (work or school account)</span></span> | <span data-ttu-id="44154-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44154-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="44154-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44154-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44154-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44154-111">Not supported.</span></span>    |
|<span data-ttu-id="44154-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44154-112">Application</span></span> | <span data-ttu-id="44154-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44154-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44154-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44154-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="44154-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44154-115">Request headers</span></span>
| <span data-ttu-id="44154-116">Nome</span><span class="sxs-lookup"><span data-stu-id="44154-116">Name</span></span>       | <span data-ttu-id="44154-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="44154-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="44154-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="44154-118">Authorization</span></span>  | <span data-ttu-id="44154-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44154-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="44154-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="44154-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="44154-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="44154-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44154-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44154-124">Request body</span></span>
<span data-ttu-id="44154-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44154-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="44154-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="44154-126">Parameter</span></span>    | <span data-ttu-id="44154-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="44154-127">Type</span></span>   |<span data-ttu-id="44154-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="44154-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44154-129">index</span><span class="sxs-lookup"><span data-stu-id="44154-129">index</span></span>|<span data-ttu-id="44154-130">number</span><span class="sxs-lookup"><span data-stu-id="44154-130">number</span></span>|<span data-ttu-id="44154-p104">Especifica a posição relativa da nova coluna. A coluna anterior nessa posição é deslocada para a direita. O valor do índice deve ser igual ou menor que o valor do índice da última coluna, portanto não pode ser usado para acrescentar uma coluna ao final da tabela. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="44154-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="44154-135">values</span><span class="sxs-lookup"><span data-stu-id="44154-135">values</span></span>|<span data-ttu-id="44154-136">(booliano, cadeia de caracteres ou número)</span><span class="sxs-lookup"><span data-stu-id="44154-136">(boolean or string or number)</span></span>|<span data-ttu-id="44154-p105">Opcional. Uma matriz bidimensional de valores não formatados da coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="44154-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="44154-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="44154-139">Response</span></span>

<span data-ttu-id="44154-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [TableColumn](../resources/tablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44154-140">If successful, this method returns `200 OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44154-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44154-141">Example</span></span>
<span data-ttu-id="44154-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="44154-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="44154-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44154-143">Request</span></span>
<span data-ttu-id="44154-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44154-144">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="44154-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="44154-145">Response</span></span>
<span data-ttu-id="44154-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44154-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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