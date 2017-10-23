# <a name="tablecolumncollection-itemat"></a><span data-ttu-id="377f9-101">TableColumnCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="377f9-101">TableColumnCollection: ItemAt</span></span>

<span data-ttu-id="377f9-102">Obtém uma coluna com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="377f9-102">Gets a column based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="377f9-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="377f9-103">Permissions</span></span>
<span data-ttu-id="377f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="377f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="377f9-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="377f9-106">Permission type</span></span>      | <span data-ttu-id="377f9-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="377f9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="377f9-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="377f9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="377f9-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="377f9-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="377f9-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="377f9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="377f9-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="377f9-111">Not supported.</span></span>    |
|<span data-ttu-id="377f9-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="377f9-112">Application</span></span> | <span data-ttu-id="377f9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="377f9-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="377f9-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="377f9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/ItemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="377f9-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="377f9-115">Request headers</span></span>
| <span data-ttu-id="377f9-116">Nome</span><span class="sxs-lookup"><span data-stu-id="377f9-116">Name</span></span>       | <span data-ttu-id="377f9-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="377f9-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="377f9-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="377f9-118">Authorization</span></span>  | <span data-ttu-id="377f9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="377f9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="377f9-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="377f9-121">Request body</span></span>
<span data-ttu-id="377f9-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="377f9-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="377f9-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="377f9-123">Parameter</span></span>    | <span data-ttu-id="377f9-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="377f9-124">Type</span></span>   |<span data-ttu-id="377f9-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="377f9-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="377f9-126">índice</span><span class="sxs-lookup"><span data-stu-id="377f9-126">index</span></span>|<span data-ttu-id="377f9-127">number</span><span class="sxs-lookup"><span data-stu-id="377f9-127">number</span></span>|<span data-ttu-id="377f9-p103">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="377f9-p103">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="377f9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="377f9-130">Response</span></span>

<span data-ttu-id="377f9-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [TableColumn](../resources/tablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="377f9-131">If successful, this method returns `200 OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="377f9-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="377f9-132">Example</span></span>
<span data-ttu-id="377f9-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="377f9-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="377f9-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="377f9-134">Request</span></span>
<span data-ttu-id="377f9-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="377f9-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="377f9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="377f9-136">Response</span></span>
<span data-ttu-id="377f9-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="377f9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumnCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->