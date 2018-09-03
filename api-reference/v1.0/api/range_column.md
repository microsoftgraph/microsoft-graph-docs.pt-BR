# <a name="range-column"></a><span data-ttu-id="f3330-101">Range: Column</span><span class="sxs-lookup"><span data-stu-id="f3330-101">Range: Column</span></span>

<span data-ttu-id="f3330-102">Obtém uma coluna incluída no intervalo.</span><span class="sxs-lookup"><span data-stu-id="f3330-102">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="f3330-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3330-103">Permissions</span></span>
<span data-ttu-id="f3330-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f3330-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f3330-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3330-106">Permission type</span></span>      | <span data-ttu-id="f3330-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3330-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3330-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3330-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f3330-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3330-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f3330-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3330-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3330-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3330-111">Not supported.</span></span>    |
|<span data-ttu-id="f3330-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3330-112">Application</span></span> | <span data-ttu-id="f3330-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3330-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3330-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3330-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/column
GET /workbook/worksheets/{id|name}/range(address='<address>')/column
GET /workbook/tables/{id|name}/columns/{id|name}/range/column

```
## <a name="request-headers"></a><span data-ttu-id="f3330-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3330-115">Request headers</span></span>
| <span data-ttu-id="f3330-116">Nome</span><span class="sxs-lookup"><span data-stu-id="f3330-116">Name</span></span>       | <span data-ttu-id="f3330-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3330-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f3330-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3330-118">Authorization</span></span>  | <span data-ttu-id="f3330-p102">Portador {token}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3330-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f3330-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f3330-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="f3330-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f3330-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="f3330-124">Parâmetros de caminho</span><span class="sxs-lookup"><span data-stu-id="f3330-124">Path parameters</span></span>
<span data-ttu-id="f3330-125">Forneça os seguintes parâmetros no caminho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3330-125">In the request URL, provide the following query parameters with values.</span></span>

| <span data-ttu-id="f3330-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f3330-126">Parameter</span></span>    | <span data-ttu-id="f3330-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3330-127">Type</span></span>   |<span data-ttu-id="f3330-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3330-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3330-129">column</span><span class="sxs-lookup"><span data-stu-id="f3330-129">column</span></span>|<span data-ttu-id="f3330-130">Int32</span><span class="sxs-lookup"><span data-stu-id="f3330-130">Int32</span></span>|<span data-ttu-id="f3330-p104">O número da coluna do intervalo a ser recuperado. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="f3330-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="f3330-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3330-133">Response</span></span>

<span data-ttu-id="f3330-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3330-134">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3330-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3330-135">Example</span></span>
<span data-ttu-id="f3330-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f3330-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f3330-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3330-137">Request</span></span>
<span data-ttu-id="f3330-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3330-138">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)
```

##### <a name="response"></a><span data-ttu-id="f3330-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3330-139">Response</span></span>
<span data-ttu-id="f3330-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3330-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->