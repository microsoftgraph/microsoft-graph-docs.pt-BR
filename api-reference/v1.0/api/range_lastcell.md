# <a name="range-lastcell"></a><span data-ttu-id="0cd79-101">Range: LastCell</span><span class="sxs-lookup"><span data-stu-id="0cd79-101">Range: LastCell</span></span>

<span data-ttu-id="0cd79-p101">Obtém a última célula do intervalo. Por exemplo, a última célula de "B2:D5" é "D5".</span><span class="sxs-lookup"><span data-stu-id="0cd79-p101">Gets the last cell within the range. For example, the last cell of "B2:D5" is "D5".</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0cd79-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0cd79-104">Prerequisites</span></span>
<span data-ttu-id="0cd79-105">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="0cd79-105">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="0cd79-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0cd79-106">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="0cd79-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cd79-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastCell
GET /workbook/worksheets/{id|name}/range(<address>)/LastCell
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastCell

```
## <a name="request-headers"></a><span data-ttu-id="0cd79-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cd79-108">Request headers</span></span>
| <span data-ttu-id="0cd79-109">Nome</span><span class="sxs-lookup"><span data-stu-id="0cd79-109">Name</span></span>       | <span data-ttu-id="0cd79-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cd79-110">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0cd79-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cd79-111">Authorization</span></span>  | <span data-ttu-id="0cd79-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0cd79-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0cd79-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cd79-114">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0cd79-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cd79-115">Response</span></span>

<span data-ttu-id="0cd79-116">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cd79-116">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cd79-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cd79-117">Example</span></span>
<span data-ttu-id="0cd79-118">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0cd79-118">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0cd79-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cd79-119">Request</span></span>
<span data-ttu-id="0cd79-120">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cd79-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastcell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/LastCell
```

##### <a name="response"></a><span data-ttu-id="0cd79-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cd79-121">Response</span></span>
<span data-ttu-id="0cd79-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0cd79-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastCell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->