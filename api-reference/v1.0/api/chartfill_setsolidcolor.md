# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="47b3d-101">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="47b3d-101">ChartFill: setSolidColor</span></span>

<span data-ttu-id="47b3d-102">Define a formatação de preenchimento de um elemento do gráfico com uma cor uniforme.</span><span class="sxs-lookup"><span data-stu-id="47b3d-102">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47b3d-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47b3d-103">Prerequisites</span></span>
<span data-ttu-id="47b3d-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="47b3d-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="47b3d-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47b3d-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="47b3d-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47b3d-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="47b3d-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47b3d-107">Request headers</span></span>
| <span data-ttu-id="47b3d-108">Nome</span><span class="sxs-lookup"><span data-stu-id="47b3d-108">Name</span></span>       | <span data-ttu-id="47b3d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="47b3d-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="47b3d-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="47b3d-110">Authorization</span></span>  | <span data-ttu-id="47b3d-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47b3d-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="47b3d-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47b3d-113">Request body</span></span>
<span data-ttu-id="47b3d-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47b3d-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="47b3d-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="47b3d-115">Parameter</span></span>    | <span data-ttu-id="47b3d-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="47b3d-116">Type</span></span>   |<span data-ttu-id="47b3d-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="47b3d-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47b3d-118">color</span><span class="sxs-lookup"><span data-stu-id="47b3d-118">color</span></span>|<span data-ttu-id="47b3d-119">string</span><span class="sxs-lookup"><span data-stu-id="47b3d-119">string</span></span>|<span data-ttu-id="47b3d-120">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="47b3d-120">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="47b3d-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="47b3d-121">Response</span></span>

<span data-ttu-id="47b3d-p102">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47b3d-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47b3d-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47b3d-124">Example</span></span>
<span data-ttu-id="47b3d-125">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="47b3d-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="47b3d-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47b3d-126">Request</span></span>
<span data-ttu-id="47b3d-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47b3d-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

##### <a name="response"></a><span data-ttu-id="47b3d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="47b3d-128">Response</span></span>
<span data-ttu-id="47b3d-129">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47b3d-129">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->