# <a name="range-insert"></a><span data-ttu-id="75351-101">Range: insert</span><span class="sxs-lookup"><span data-stu-id="75351-101">Range: insert</span></span>

<span data-ttu-id="75351-p101">Insere uma célula ou um intervalo de células na planilha, no lugar desse intervalo, e desloca as outras células para liberar espaço. Retorna um novo objeto Range no espaço em branco atual.</span><span class="sxs-lookup"><span data-stu-id="75351-p101">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="75351-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="75351-104">Permissions</span></span>
<span data-ttu-id="75351-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="75351-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="75351-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75351-107">Permission type</span></span>      | <span data-ttu-id="75351-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75351-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75351-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75351-109">Delegated (work or school account)</span></span> | <span data-ttu-id="75351-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75351-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75351-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75351-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75351-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75351-112">Not supported.</span></span>    |
|<span data-ttu-id="75351-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75351-113">Application</span></span> | <span data-ttu-id="75351-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75351-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75351-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75351-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="75351-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75351-116">Request headers</span></span>
| <span data-ttu-id="75351-117">Nome</span><span class="sxs-lookup"><span data-stu-id="75351-117">Name</span></span>       | <span data-ttu-id="75351-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="75351-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="75351-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="75351-119">Authorization</span></span>  | <span data-ttu-id="75351-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75351-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="75351-122">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="75351-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="75351-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="75351-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75351-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75351-125">Request body</span></span>
<span data-ttu-id="75351-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75351-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="75351-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="75351-127">Parameter</span></span>    | <span data-ttu-id="75351-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="75351-128">Type</span></span>   |<span data-ttu-id="75351-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="75351-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75351-130">shift</span><span class="sxs-lookup"><span data-stu-id="75351-130">shift</span></span>|<span data-ttu-id="75351-131">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="75351-131">string</span></span>|<span data-ttu-id="75351-132">Especifica como deslocar as células.</span><span class="sxs-lookup"><span data-stu-id="75351-132">Specifies which way to shift the cells.  Possible values are: Down, Right</span></span>  <span data-ttu-id="75351-133">Os valores possíveis são: `Down`, `Right`.</span><span class="sxs-lookup"><span data-stu-id="75351-133">The possible values are:</span></span>|

## <a name="response"></a><span data-ttu-id="75351-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="75351-134">Response</span></span>

<span data-ttu-id="75351-135">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75351-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75351-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75351-136">Example</span></span>
<span data-ttu-id="75351-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="75351-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="75351-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75351-138">Request</span></span>
<span data-ttu-id="75351-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75351-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="75351-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="75351-140">Response</span></span>
<span data-ttu-id="75351-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75351-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->