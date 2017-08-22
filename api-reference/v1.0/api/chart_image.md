# <a name="chart-image"></a><span data-ttu-id="facf4-101">Chart: Image</span><span class="sxs-lookup"><span data-stu-id="facf4-101">Chart: Image</span></span>

<span data-ttu-id="facf4-102">Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.</span><span class="sxs-lookup"><span data-stu-id="facf4-102">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="facf4-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="facf4-103">Prerequisites</span></span>
<span data-ttu-id="facf4-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="facf4-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="facf4-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="facf4-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="facf4-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="facf4-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="facf4-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="facf4-107">Request headers</span></span>
| <span data-ttu-id="facf4-108">Nome</span><span class="sxs-lookup"><span data-stu-id="facf4-108">Name</span></span>       | <span data-ttu-id="facf4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="facf4-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="facf4-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="facf4-110">Authorization</span></span>  | <span data-ttu-id="facf4-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="facf4-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="facf4-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="facf4-113">Request body</span></span>
<span data-ttu-id="facf4-114">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="facf4-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="facf4-115">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="facf4-115">Parameter</span></span>    | <span data-ttu-id="facf4-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="facf4-116">Type</span></span>   |<span data-ttu-id="facf4-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="facf4-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="facf4-118">height</span><span class="sxs-lookup"><span data-stu-id="facf4-118">height</span></span>|<span data-ttu-id="facf4-119">number</span><span class="sxs-lookup"><span data-stu-id="facf4-119">number</span></span>|<span data-ttu-id="facf4-p102">Opcional. A altura desejada da imagem resultante.</span><span class="sxs-lookup"><span data-stu-id="facf4-p102">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="facf4-122">width</span><span class="sxs-lookup"><span data-stu-id="facf4-122">width</span></span>|<span data-ttu-id="facf4-123">number</span><span class="sxs-lookup"><span data-stu-id="facf4-123">number</span></span>|<span data-ttu-id="facf4-p103">Opcional. A largura desejada da imagem resultante.</span><span class="sxs-lookup"><span data-stu-id="facf4-p103">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="facf4-126">fittingMode</span><span class="sxs-lookup"><span data-stu-id="facf4-126">fittingMode</span></span>|<span data-ttu-id="facf4-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="facf4-127">string</span></span>|<span data-ttu-id="facf4-p104">Opcional. O método usado para dimensionar o gráfico para as dimensões especificadas (se height e width tiverem sido definidas).  Os valores possíveis são: `Fit`, `FitAndCenter` e `Fill`.</span><span class="sxs-lookup"><span data-stu-id="facf4-p104">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="facf4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="facf4-131">Response</span></span>

<span data-ttu-id="facf4-132">Se bem-sucedido, este método retorna o código de resposta `200, OK` e a cadeia de caracteres de imagem em base64 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="facf4-132">If successful, this method returns `200, OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="facf4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="facf4-133">Example</span></span>
<span data-ttu-id="facf4-134">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="facf4-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="facf4-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="facf4-135">Request</span></span>
<span data-ttu-id="facf4-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="facf4-136">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
Content-type: application/json
Content-length: 77

{
  "height": {
  },
  "width": {
  },
  "fittingMode": "fittingMode-value"
}
```

##### <a name="response"></a><span data-ttu-id="facf4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="facf4-137">Response</span></span>
<span data-ttu-id="facf4-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="facf4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
