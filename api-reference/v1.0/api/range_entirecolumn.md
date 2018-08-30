# <a name="range-entirecolumn"></a><span data-ttu-id="64c7c-101">Intervalo: EntireColumn</span><span class="sxs-lookup"><span data-stu-id="64c7c-101">Range: EntireColumn</span></span>

<span data-ttu-id="64c7c-102">Obtém um objeto que representa toda a coluna do intervalo.</span><span class="sxs-lookup"><span data-stu-id="64c7c-102">Gets an object that represents the entire column of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="64c7c-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="64c7c-103">Permissions</span></span>
<span data-ttu-id="64c7c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="64c7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="64c7c-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64c7c-106">Permission type</span></span>      | <span data-ttu-id="64c7c-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64c7c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64c7c-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64c7c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="64c7c-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64c7c-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="64c7c-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64c7c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64c7c-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64c7c-111">Not supported.</span></span>    |
|<span data-ttu-id="64c7c-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64c7c-112">Application</span></span> | <span data-ttu-id="64c7c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64c7c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64c7c-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64c7c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/entireColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/entireColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/entireColumn

```
## <a name="request-headers"></a><span data-ttu-id="64c7c-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64c7c-115">Request headers</span></span>
| <span data-ttu-id="64c7c-116">Nome</span><span class="sxs-lookup"><span data-stu-id="64c7c-116">Name</span></span>       | <span data-ttu-id="64c7c-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="64c7c-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="64c7c-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="64c7c-118">Authorization</span></span>  | <span data-ttu-id="64c7c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64c7c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="64c7c-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="64c7c-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="64c7c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="64c7c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64c7c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64c7c-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="64c7c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="64c7c-125">Response</span></span>

<span data-ttu-id="64c7c-126">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64c7c-126">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64c7c-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64c7c-127">Example</span></span>
<span data-ttu-id="64c7c-128">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="64c7c-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="64c7c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64c7c-129">Request</span></span>
<span data-ttu-id="64c7c-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64c7c-130">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_entirecolumn"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/entireColumn
```

##### <a name="response"></a><span data-ttu-id="64c7c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="64c7c-131">Response</span></span>
<span data-ttu-id="64c7c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64c7c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: EntireColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->