# <a name="tablecolumncollection-itemat"></a><span data-ttu-id="e6f23-101">TableColumnCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="e6f23-101">TableColumnCollection: ItemAt</span></span>

<span data-ttu-id="e6f23-102">Obtém uma coluna com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="e6f23-102">Gets a column based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="e6f23-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6f23-103">Permissions</span></span>
<span data-ttu-id="e6f23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e6f23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e6f23-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6f23-106">Permission type</span></span>      | <span data-ttu-id="e6f23-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6f23-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6f23-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6f23-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e6f23-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6f23-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e6f23-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6f23-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6f23-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6f23-111">Not supported.</span></span>    |
|<span data-ttu-id="e6f23-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6f23-112">Application</span></span> | <span data-ttu-id="e6f23-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6f23-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6f23-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6f23-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/itemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="e6f23-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6f23-115">Request headers</span></span>
| <span data-ttu-id="e6f23-116">Nome</span><span class="sxs-lookup"><span data-stu-id="e6f23-116">Name</span></span>       | <span data-ttu-id="e6f23-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6f23-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e6f23-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6f23-118">Authorization</span></span>  | <span data-ttu-id="e6f23-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6f23-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e6f23-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e6f23-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="e6f23-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e6f23-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6f23-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6f23-124">Request body</span></span>
<span data-ttu-id="e6f23-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6f23-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e6f23-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e6f23-126">Parameter</span></span>    | <span data-ttu-id="e6f23-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6f23-127">Type</span></span>   |<span data-ttu-id="e6f23-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6f23-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6f23-129">índice</span><span class="sxs-lookup"><span data-stu-id="e6f23-129">index</span></span>|<span data-ttu-id="e6f23-130">Int32</span><span class="sxs-lookup"><span data-stu-id="e6f23-130">Int32</span></span>|<span data-ttu-id="e6f23-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="e6f23-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="e6f23-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6f23-133">Response</span></span>

<span data-ttu-id="e6f23-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [WorkbookTableColumn](../resources/tablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6f23-134">If successful, this method returns `200 OK` response code and [groupSetting](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6f23-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6f23-135">Example</span></span>
<span data-ttu-id="e6f23-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e6f23-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e6f23-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6f23-137">Request</span></span>
<span data-ttu-id="e6f23-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6f23-138">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumncollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.tablecolumncollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 3
}
```

##### <a name="response"></a><span data-ttu-id="e6f23-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6f23-139">Response</span></span>
<span data-ttu-id="e6f23-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6f23-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
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