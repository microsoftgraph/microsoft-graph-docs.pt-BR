# <a name="tablerowcollection-itemat"></a><span data-ttu-id="eac07-101">TableRowCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="eac07-101">TableRowCollection: ItemAt</span></span>

<span data-ttu-id="eac07-102">Obtém uma linha com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="eac07-102">Gets a row based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="eac07-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="eac07-103">Permissions</span></span>
<span data-ttu-id="eac07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eac07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eac07-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eac07-106">Permission type</span></span>      | <span data-ttu-id="eac07-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eac07-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eac07-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eac07-108">Delegated (work or school account)</span></span> | <span data-ttu-id="eac07-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eac07-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eac07-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eac07-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eac07-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eac07-111">Not supported.</span></span>    |
|<span data-ttu-id="eac07-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eac07-112">Application</span></span> | <span data-ttu-id="eac07-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eac07-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eac07-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eac07-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/ItemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="eac07-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eac07-115">Request headers</span></span>
| <span data-ttu-id="eac07-116">Nome</span><span class="sxs-lookup"><span data-stu-id="eac07-116">Name</span></span>       | <span data-ttu-id="eac07-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="eac07-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eac07-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="eac07-118">Authorization</span></span>  | <span data-ttu-id="eac07-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eac07-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eac07-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="eac07-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="eac07-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="eac07-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eac07-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eac07-124">Request body</span></span>
<span data-ttu-id="eac07-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eac07-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eac07-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="eac07-126">Parameter</span></span>    | <span data-ttu-id="eac07-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="eac07-127">Type</span></span>   |<span data-ttu-id="eac07-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="eac07-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eac07-129">index</span><span class="sxs-lookup"><span data-stu-id="eac07-129">index</span></span>|<span data-ttu-id="eac07-130">number</span><span class="sxs-lookup"><span data-stu-id="eac07-130">number</span></span>|<span data-ttu-id="eac07-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="eac07-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="eac07-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="eac07-133">Response</span></span>

<span data-ttu-id="eac07-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [TableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eac07-134">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eac07-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eac07-135">Example</span></span>
<span data-ttu-id="eac07-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="eac07-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eac07-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eac07-137">Request</span></span>
<span data-ttu-id="eac07-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eac07-138">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="eac07-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="eac07-139">Response</span></span>
<span data-ttu-id="eac07-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eac07-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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