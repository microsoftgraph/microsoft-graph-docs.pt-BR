# <a name="worksheet-cell"></a><span data-ttu-id="f5ecd-101">Worksheet: Cell</span><span class="sxs-lookup"><span data-stu-id="f5ecd-101">Worksheet: Cell</span></span>

<span data-ttu-id="f5ecd-p101">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha.</span><span class="sxs-lookup"><span data-stu-id="f5ecd-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f5ecd-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5ecd-104">Prerequisites</span></span>
<span data-ttu-id="f5ecd-105">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="f5ecd-105">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="f5ecd-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5ecd-106">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="f5ecd-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5ecd-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)

```
## <a name="request-headers"></a><span data-ttu-id="f5ecd-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ecd-108">Request headers</span></span>
| <span data-ttu-id="f5ecd-109">Nome</span><span class="sxs-lookup"><span data-stu-id="f5ecd-109">Name</span></span>       | <span data-ttu-id="f5ecd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5ecd-110">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f5ecd-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5ecd-111">Authorization</span></span>  | <span data-ttu-id="f5ecd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5ecd-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f5ecd-114">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5ecd-114">Response</span></span>

<span data-ttu-id="f5ecd-115">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5ecd-115">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5ecd-116">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5ecd-116">Example</span></span>
<span data-ttu-id="f5ecd-117">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f5ecd-117">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f5ecd-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ecd-118">Request</span></span>
<span data-ttu-id="f5ecd-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5ecd-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="f5ecd-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5ecd-120">Response</span></span>
<span data-ttu-id="f5ecd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5ecd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
