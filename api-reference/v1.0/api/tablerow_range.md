# <a name="tablerow-range"></a><span data-ttu-id="ca6f6-101">TableRow: Range</span><span class="sxs-lookup"><span data-stu-id="ca6f6-101">TableRow: Range</span></span>

<span data-ttu-id="ca6f6-102">Retorna o objeto de intervalo associado a toda a linha.</span><span class="sxs-lookup"><span data-stu-id="ca6f6-102">Returns the range object associated with the entire row.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca6f6-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca6f6-103">Prerequisites</span></span>
<span data-ttu-id="ca6f6-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="ca6f6-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="ca6f6-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca6f6-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="ca6f6-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca6f6-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows(<index>)/Range
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)/Range

```
## <a name="request-headers"></a><span data-ttu-id="ca6f6-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca6f6-107">Request headers</span></span>
| <span data-ttu-id="ca6f6-108">Nome</span><span class="sxs-lookup"><span data-stu-id="ca6f6-108">Name</span></span>       | <span data-ttu-id="ca6f6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca6f6-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ca6f6-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca6f6-110">Authorization</span></span>  | <span data-ttu-id="ca6f6-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca6f6-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="ca6f6-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca6f6-113">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ca6f6-114">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca6f6-114">Response</span></span>

<span data-ttu-id="ca6f6-115">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca6f6-115">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca6f6-116">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca6f6-116">Example</span></span>
<span data-ttu-id="ca6f6-117">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ca6f6-117">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ca6f6-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca6f6-118">Request</span></span>
<span data-ttu-id="ca6f6-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca6f6-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)/Range
```

##### <a name="response"></a><span data-ttu-id="ca6f6-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca6f6-120">Response</span></span>
<span data-ttu-id="ca6f6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca6f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableRow: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->