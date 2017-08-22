# <a name="worksheet-range"></a><span data-ttu-id="53944-101">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="53944-101">Worksheet: Range</span></span>

<span data-ttu-id="53944-102">Obtém o objeto de intervalo especificado pelo nome ou endereço.</span><span class="sxs-lookup"><span data-stu-id="53944-102">Gets the range object specified by the address or name.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53944-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53944-103">Prerequisites</span></span>
<span data-ttu-id="53944-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="53944-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="53944-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53944-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="53944-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53944-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="53944-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53944-107">Request headers</span></span>
| <span data-ttu-id="53944-108">Nome</span><span class="sxs-lookup"><span data-stu-id="53944-108">Name</span></span>       | <span data-ttu-id="53944-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="53944-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="53944-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="53944-110">Authorization</span></span>  | <span data-ttu-id="53944-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53944-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="53944-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53944-113">Request body</span></span>
<span data-ttu-id="53944-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53944-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="53944-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="53944-115">Parameter</span></span>    | <span data-ttu-id="53944-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="53944-116">Type</span></span>   |<span data-ttu-id="53944-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="53944-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53944-118">address</span><span class="sxs-lookup"><span data-stu-id="53944-118">address</span></span>|<span data-ttu-id="53944-119">string</span><span class="sxs-lookup"><span data-stu-id="53944-119">string</span></span>|<span data-ttu-id="53944-p102">Opcional. O endereço ou nome do intervalo. Caso não seja especificado, todo o intervalo da planilha será retornado.</span><span class="sxs-lookup"><span data-stu-id="53944-p102">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="53944-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="53944-123">Response</span></span>

<span data-ttu-id="53944-124">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53944-124">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53944-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53944-125">Example</span></span>
<span data-ttu-id="53944-126">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="53944-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="53944-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53944-127">Request</span></span>
<span data-ttu-id="53944-128">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53944-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```

##### <a name="response"></a><span data-ttu-id="53944-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="53944-129">Response</span></span>
<span data-ttu-id="53944-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53944-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->