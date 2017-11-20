# <a name="range-lastcolumn"></a><span data-ttu-id="6b9c4-101">Range: LastColumn</span><span class="sxs-lookup"><span data-stu-id="6b9c4-101">Range: LastColumn</span></span>

<span data-ttu-id="6b9c4-p101">Obtém a última coluna do intervalo. Por exemplo, a última coluna de "B2:D5" é "D2:D5".</span><span class="sxs-lookup"><span data-stu-id="6b9c4-p101">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="6b9c4-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b9c4-104">Permissions</span></span>
<span data-ttu-id="6b9c4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6b9c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6b9c4-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b9c4-107">Permission type</span></span>      | <span data-ttu-id="6b9c4-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b9c4-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b9c4-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b9c4-109">Delegated (work or school account)</span></span> | <span data-ttu-id="6b9c4-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b9c4-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6b9c4-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b9c4-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b9c4-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b9c4-112">Not supported.</span></span>    |
|<span data-ttu-id="6b9c4-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b9c4-113">Application</span></span> | <span data-ttu-id="6b9c4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b9c4-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b9c4-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b9c4-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastColumn

```
## <a name="request-headers"></a><span data-ttu-id="6b9c4-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b9c4-116">Request headers</span></span>
| <span data-ttu-id="6b9c4-117">Nome</span><span class="sxs-lookup"><span data-stu-id="6b9c4-117">Name</span></span>       | <span data-ttu-id="6b9c4-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b9c4-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6b9c4-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b9c4-119">Authorization</span></span>  | <span data-ttu-id="6b9c4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b9c4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6b9c4-122">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6b9c4-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="6b9c4-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="6b9c4-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b9c4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b9c4-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="6b9c4-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b9c4-126">Response</span></span>

<span data-ttu-id="6b9c4-127">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b9c4-127">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b9c4-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b9c4-128">Example</span></span>
<span data-ttu-id="6b9c4-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6b9c4-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6b9c4-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b9c4-130">Request</span></span>
<span data-ttu-id="6b9c4-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b9c4-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastcolumn"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/LastColumn
```

##### <a name="response"></a><span data-ttu-id="6b9c4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b9c4-132">Response</span></span>
<span data-ttu-id="6b9c4-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b9c4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
  "description": "Range: LastColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->