# <a name="tablecolumncollection-add"></a><span data-ttu-id="5dc78-101">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="5dc78-101">TableColumnCollection: add</span></span>

<span data-ttu-id="5dc78-102">Adiciona uma nova coluna à tabela.</span><span class="sxs-lookup"><span data-stu-id="5dc78-102">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="5dc78-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="5dc78-103">Permissions</span></span>
<span data-ttu-id="5dc78-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5dc78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5dc78-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dc78-106">Permission type</span></span>      | <span data-ttu-id="5dc78-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5dc78-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5dc78-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dc78-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5dc78-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5dc78-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5dc78-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dc78-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dc78-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dc78-111">Not supported.</span></span>    |
|<span data-ttu-id="5dc78-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dc78-112">Application</span></span> | <span data-ttu-id="5dc78-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dc78-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5dc78-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dc78-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="5dc78-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc78-115">Request headers</span></span>
| <span data-ttu-id="5dc78-116">Nome</span><span class="sxs-lookup"><span data-stu-id="5dc78-116">Name</span></span>       | <span data-ttu-id="5dc78-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dc78-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5dc78-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dc78-118">Authorization</span></span>  | <span data-ttu-id="5dc78-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dc78-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5dc78-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc78-121">Request body</span></span>
<span data-ttu-id="5dc78-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dc78-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5dc78-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5dc78-123">Parameter</span></span>    | <span data-ttu-id="5dc78-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dc78-124">Type</span></span>   |<span data-ttu-id="5dc78-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dc78-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5dc78-126">índice</span><span class="sxs-lookup"><span data-stu-id="5dc78-126">index</span></span>|<span data-ttu-id="5dc78-127">number</span><span class="sxs-lookup"><span data-stu-id="5dc78-127">number</span></span>|<span data-ttu-id="5dc78-p103">Especifica a posição relativa da nova coluna. A coluna anterior nessa posição é deslocada para a direita. O valor do índice deve ser igual ou menor que o valor do índice da última coluna, portanto não pode ser usado para acrescentar uma coluna ao final da tabela. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="5dc78-p103">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="5dc78-132">values</span><span class="sxs-lookup"><span data-stu-id="5dc78-132">values</span></span>|<span data-ttu-id="5dc78-133">(booliano, cadeia de caracteres ou número)</span><span class="sxs-lookup"><span data-stu-id="5dc78-133">(boolean or string or number)</span></span>|<span data-ttu-id="5dc78-p104">Opcional. Uma matriz bidimensional de valores não formatados da coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="5dc78-p104">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="5dc78-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc78-136">Response</span></span>

<span data-ttu-id="5dc78-137">Se bem-sucedido, este método retorna um código de resposta `200, OK` e um objeto [TableColumn](../resources/tablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dc78-137">If successful, this method returns `200, OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dc78-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dc78-138">Example</span></span>
<span data-ttu-id="5dc78-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5dc78-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5dc78-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc78-140">Request</span></span>
<span data-ttu-id="5dc78-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dc78-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="5dc78-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc78-142">Response</span></span>
<span data-ttu-id="5dc78-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5dc78-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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