# <a name="worksheet-cell"></a><span data-ttu-id="1d16f-101">Worksheet: Cell</span><span class="sxs-lookup"><span data-stu-id="1d16f-101">Worksheet: Cell</span></span>

<span data-ttu-id="1d16f-p101">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha.</span><span class="sxs-lookup"><span data-stu-id="1d16f-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d16f-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d16f-104">Permissions</span></span>
<span data-ttu-id="1d16f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1d16f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1d16f-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d16f-107">Permission type</span></span>      | <span data-ttu-id="1d16f-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d16f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d16f-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d16f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="1d16f-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d16f-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1d16f-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d16f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d16f-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d16f-112">Not supported.</span></span>    |
|<span data-ttu-id="1d16f-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d16f-113">Application</span></span> | <span data-ttu-id="1d16f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d16f-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d16f-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d16f-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)

```
## <a name="request-headers"></a><span data-ttu-id="1d16f-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d16f-116">Request headers</span></span>
| <span data-ttu-id="1d16f-117">Nome</span><span class="sxs-lookup"><span data-stu-id="1d16f-117">Name</span></span>       | <span data-ttu-id="1d16f-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d16f-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1d16f-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d16f-119">Authorization</span></span>  | <span data-ttu-id="1d16f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d16f-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1d16f-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d16f-122">Response</span></span>

<span data-ttu-id="1d16f-123">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d16f-123">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d16f-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d16f-124">Example</span></span>
<span data-ttu-id="1d16f-125">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1d16f-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1d16f-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d16f-126">Request</span></span>
<span data-ttu-id="1d16f-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d16f-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="1d16f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d16f-128">Response</span></span>
<span data-ttu-id="1d16f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d16f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "cellCount": 1,
  "columnCount": 1,
  "columnIndex": 3,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
