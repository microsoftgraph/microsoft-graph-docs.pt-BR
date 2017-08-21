# <a name="worksheet-usedrange"></a><span data-ttu-id="86547-101">Worksheet: UsedRange</span><span class="sxs-lookup"><span data-stu-id="86547-101">Worksheet: UsedRange</span></span>

<span data-ttu-id="86547-p101">O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.</span><span class="sxs-lookup"><span data-stu-id="86547-p101">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86547-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86547-104">Prerequisites</span></span>
<span data-ttu-id="86547-105">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="86547-105">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="86547-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86547-106">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="86547-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86547-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/UsedRange

```

## <a name="optional-request-parameter"></a><span data-ttu-id="86547-108">Parâmetro de solicitação opcional</span><span class="sxs-lookup"><span data-stu-id="86547-108">Optional request parameter</span></span>
<span data-ttu-id="86547-109">No URL de solicitação, forneça um parâmetro de consulta opcional.</span><span class="sxs-lookup"><span data-stu-id="86547-109">In the request URL, provide an optional query parameter.</span></span>

| <span data-ttu-id="86547-110">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="86547-110">Parameter</span></span>    | <span data-ttu-id="86547-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="86547-111">Type</span></span>   |<span data-ttu-id="86547-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="86547-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86547-113">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="86547-113">valuesOnly</span></span>|<span data-ttu-id="86547-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="86547-114">Boolean</span></span>|<span data-ttu-id="86547-p102">Opcional. Considera apenas as células com valores como células usadas (ignora a formatação).</span><span class="sxs-lookup"><span data-stu-id="86547-p102">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|


## <a name="request-headers"></a><span data-ttu-id="86547-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86547-117">Request headers</span></span>
| <span data-ttu-id="86547-118">Nome</span><span class="sxs-lookup"><span data-stu-id="86547-118">Name</span></span>       | <span data-ttu-id="86547-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="86547-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="86547-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="86547-120">Authorization</span></span>  | <span data-ttu-id="86547-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86547-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="86547-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="86547-123">Response</span></span>

<span data-ttu-id="86547-124">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86547-124">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86547-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86547-125">Example</span></span>
<span data-ttu-id="86547-126">Aqui está um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="86547-126">Here is an example that shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="86547-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86547-127">Request</span></span>
<span data-ttu-id="86547-128">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86547-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)
Content-type: application/json

```

##### <a name="response"></a><span data-ttu-id="86547-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="86547-129">Response</span></span>
<span data-ttu-id="86547-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86547-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
