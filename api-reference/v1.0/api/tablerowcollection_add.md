# <a name="tablerowcollection-add"></a><span data-ttu-id="baf2a-101">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="baf2a-101">TableRowCollection: add</span></span>

<span data-ttu-id="baf2a-102">Adiciona uma nova linha à tabela.</span><span class="sxs-lookup"><span data-stu-id="baf2a-102">Adds a new row to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="baf2a-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="baf2a-103">Permissions</span></span>
<span data-ttu-id="baf2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="baf2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="baf2a-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="baf2a-106">Permission type</span></span>      | <span data-ttu-id="baf2a-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="baf2a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="baf2a-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="baf2a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="baf2a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="baf2a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="baf2a-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="baf2a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baf2a-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="baf2a-111">Not supported.</span></span>    |
|<span data-ttu-id="baf2a-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="baf2a-112">Application</span></span> | <span data-ttu-id="baf2a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="baf2a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="baf2a-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="baf2a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="baf2a-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="baf2a-115">Request headers</span></span>
| <span data-ttu-id="baf2a-116">Nome</span><span class="sxs-lookup"><span data-stu-id="baf2a-116">Name</span></span>       | <span data-ttu-id="baf2a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="baf2a-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="baf2a-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="baf2a-118">Authorization</span></span>  | <span data-ttu-id="baf2a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="baf2a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="baf2a-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="baf2a-121">Request body</span></span>
<span data-ttu-id="baf2a-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="baf2a-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="baf2a-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="baf2a-123">Parameter</span></span>    | <span data-ttu-id="baf2a-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="baf2a-124">Type</span></span>   |<span data-ttu-id="baf2a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="baf2a-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="baf2a-126">índice</span><span class="sxs-lookup"><span data-stu-id="baf2a-126">index</span></span>|<span data-ttu-id="baf2a-127">number</span><span class="sxs-lookup"><span data-stu-id="baf2a-127">number</span></span>|<span data-ttu-id="baf2a-p103">Opcional. Especifica a posição relativa da nova linha. Se for nulo, a adição ocorre no final. Todas as linhas abaixo da linha inserida serão deslocadas para baixo. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="baf2a-p103">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="baf2a-133">values</span><span class="sxs-lookup"><span data-stu-id="baf2a-133">values</span></span>|<span data-ttu-id="baf2a-134">(booliano, cadeia de caracteres ou número)</span><span class="sxs-lookup"><span data-stu-id="baf2a-134">(boolean or string or number)</span></span>|<span data-ttu-id="baf2a-p104">Opcional. Uma matriz bidimensional de valores não formatados da linha da tabela.</span><span class="sxs-lookup"><span data-stu-id="baf2a-p104">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="baf2a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="baf2a-137">Response</span></span>

<span data-ttu-id="baf2a-138">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [TableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="baf2a-138">If successful, this method returns `200, OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baf2a-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="baf2a-139">Example</span></span>
<span data-ttu-id="baf2a-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="baf2a-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="baf2a-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="baf2a-141">Request</span></span>
<span data-ttu-id="baf2a-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="baf2a-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="baf2a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="baf2a-143">Response</span></span>
<span data-ttu-id="baf2a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="baf2a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
