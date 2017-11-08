# <a name="chart-image"></a><span data-ttu-id="f0747-101">Chart: Image</span><span class="sxs-lookup"><span data-stu-id="f0747-101">Chart: Image</span></span>

<span data-ttu-id="f0747-102">Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.</span><span class="sxs-lookup"><span data-stu-id="f0747-102">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="f0747-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0747-103">Permissions</span></span>
<span data-ttu-id="f0747-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f0747-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f0747-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0747-106">Permission type</span></span>      | <span data-ttu-id="f0747-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0747-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0747-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0747-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f0747-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0747-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f0747-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0747-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0747-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0747-111">Not supported.</span></span>    |
|<span data-ttu-id="f0747-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0747-112">Application</span></span> | <span data-ttu-id="f0747-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0747-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0747-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0747-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="f0747-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0747-115">Request headers</span></span>
| <span data-ttu-id="f0747-116">Nome</span><span class="sxs-lookup"><span data-stu-id="f0747-116">Name</span></span>       | <span data-ttu-id="f0747-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0747-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f0747-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0747-118">Authorization</span></span>  | <span data-ttu-id="f0747-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0747-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0747-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0747-121">Request body</span></span>
<span data-ttu-id="f0747-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0747-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f0747-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f0747-123">Parameter</span></span>    | <span data-ttu-id="f0747-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0747-124">Type</span></span>   |<span data-ttu-id="f0747-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0747-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0747-126">height</span><span class="sxs-lookup"><span data-stu-id="f0747-126">height</span></span>|<span data-ttu-id="f0747-127">number</span><span class="sxs-lookup"><span data-stu-id="f0747-127">number</span></span>|<span data-ttu-id="f0747-p103">Opcional. A altura desejada da imagem resultante.</span><span class="sxs-lookup"><span data-stu-id="f0747-p103">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="f0747-130">width</span><span class="sxs-lookup"><span data-stu-id="f0747-130">width</span></span>|<span data-ttu-id="f0747-131">number</span><span class="sxs-lookup"><span data-stu-id="f0747-131">number</span></span>|<span data-ttu-id="f0747-p104">Opcional. A largura desejada da imagem resultante.</span><span class="sxs-lookup"><span data-stu-id="f0747-p104">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="f0747-134">fittingMode</span><span class="sxs-lookup"><span data-stu-id="f0747-134">fittingMode</span></span>|<span data-ttu-id="f0747-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0747-135">string</span></span>|<span data-ttu-id="f0747-p105">Opcional. O método usado para dimensionar o gráfico para as dimensões especificadas (se height e width tiverem sido definidas)."  Os valores possíveis são: `Fit`, `FitAndCenter` e `Fill`.</span><span class="sxs-lookup"><span data-stu-id="f0747-p105">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="f0747-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0747-139">Response</span></span>

<span data-ttu-id="f0747-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e a cadeia de caracteres de imagem em base64 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0747-140">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0747-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0747-141">Example</span></span>
<span data-ttu-id="f0747-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f0747-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f0747-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0747-143">Request</span></span>
<span data-ttu-id="f0747-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0747-144">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="f0747-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0747-145">Response</span></span>
<span data-ttu-id="f0747-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0747-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json;odata.metadata=minimal;odata.streaming=true

{
"value" : "base-64 chart image string"
}
```

## <a name="usage"></a><span data-ttu-id="f0747-149">Uso</span><span class="sxs-lookup"><span data-stu-id="f0747-149">Usage</span></span>

<span data-ttu-id="f0747-150">Você pode exibir a cadeia de caracteres Base64 dentro de uma marca de imagem HTML: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="f0747-150">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="f0747-151">Para o comportamento padrão, use `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="f0747-151">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="f0747-152">Veja um exemplo de uma imagem de gráfico retornada com os parâmetros padrão.</span><span class="sxs-lookup"><span data-stu-id="f0747-152">Here is an example of a chart image returned with the default parameters.</span></span>

![A imagem de gráfico do Excel com altura e largura padrão.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="f0747-154">Se você quiser personalizar a exibição da imagem, especifique uma altura, largura e um modo de ajuste.</span><span class="sxs-lookup"><span data-stu-id="f0747-154">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="f0747-155">Esta é a aparência da imagem do gráfico quando você a recupera com esses parâmetros: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="f0747-155">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

![A imagem de gráfico do Excel com altura e largura padrão.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-fill.png)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
