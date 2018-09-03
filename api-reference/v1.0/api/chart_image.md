# <a name="chart-image"></a><span data-ttu-id="8460a-101">Gráfico: Imagem</span><span class="sxs-lookup"><span data-stu-id="8460a-101">Chart: Image</span></span>

<span data-ttu-id="8460a-102">Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.</span><span class="sxs-lookup"><span data-stu-id="8460a-102">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="8460a-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="8460a-103">Permissions</span></span>
<span data-ttu-id="8460a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8460a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8460a-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8460a-106">Permission type</span></span>      | <span data-ttu-id="8460a-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8460a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8460a-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8460a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8460a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8460a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8460a-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8460a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8460a-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8460a-111">Not supported.</span></span>    |
|<span data-ttu-id="8460a-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8460a-112">Application</span></span> | <span data-ttu-id="8460a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8460a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8460a-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8460a-114">HTTP request</span></span>
<!-- { "blockType": "samples" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/image
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```
## <a name="request-headers"></a><span data-ttu-id="8460a-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8460a-115">Request headers</span></span>
| <span data-ttu-id="8460a-116">Nome</span><span class="sxs-lookup"><span data-stu-id="8460a-116">Name</span></span>       | <span data-ttu-id="8460a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="8460a-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8460a-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="8460a-118">Authorization</span></span>  | <span data-ttu-id="8460a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8460a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8460a-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8460a-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="8460a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="8460a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="8460a-124">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="8460a-124">Path parameters</span></span>
<span data-ttu-id="8460a-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8460a-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8460a-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8460a-126">Parameter</span></span>    | <span data-ttu-id="8460a-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8460a-127">Type</span></span>   |<span data-ttu-id="8460a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8460a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8460a-129">height</span><span class="sxs-lookup"><span data-stu-id="8460a-129">height</span></span>|<span data-ttu-id="8460a-130">Int32</span><span class="sxs-lookup"><span data-stu-id="8460a-130">Int32</span></span>|<span data-ttu-id="8460a-131">A altura desejada da imagem resultante.</span><span class="sxs-lookup"><span data-stu-id="8460a-131">Optional. The desired height of the resulting image.</span></span> <span data-ttu-id="8460a-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8460a-132">Optional.</span></span>|
|<span data-ttu-id="8460a-133">width</span><span class="sxs-lookup"><span data-stu-id="8460a-133">width</span></span>|<span data-ttu-id="8460a-134">Int32</span><span class="sxs-lookup"><span data-stu-id="8460a-134">Int32</span></span>|<span data-ttu-id="8460a-135">A largura desejada da imagem resultante.</span><span class="sxs-lookup"><span data-stu-id="8460a-135">Optional. The desired width of the resulting image.</span></span> <span data-ttu-id="8460a-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8460a-136">Optional.</span></span>|
|<span data-ttu-id="8460a-137">fittingMode</span><span class="sxs-lookup"><span data-stu-id="8460a-137">fittingMode</span></span>|<span data-ttu-id="8460a-138">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="8460a-138">string</span></span>|<span data-ttu-id="8460a-139">O método usado para dimensionar o gráfico para as dimensões especificadas (se a altura e largura estiverem definidas)."</span><span class="sxs-lookup"><span data-stu-id="8460a-139">Optional. The method used to scale the chart to the specified dimensions (if both height and width are set)."  Possible values are: , , .</span></span>  <span data-ttu-id="8460a-140">Os valores possíveis são: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="8460a-140">The possible values are:</span></span>|

## <a name="response"></a><span data-ttu-id="8460a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8460a-141">Response</span></span>

<span data-ttu-id="8460a-142">Se bem-sucedido, este método retorna o código de resposta `200 OK` e a cadeia de caracteres de imagem em base64 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8460a-142">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8460a-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8460a-143">Example</span></span>
<span data-ttu-id="8460a-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8460a-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8460a-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8460a-145">Request</span></span>
<span data-ttu-id="8460a-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8460a-146">Here is an example of the request.</span></span>

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="8460a-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="8460a-147">Response</span></span>
<span data-ttu-id="8460a-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8460a-148">Here is an example of the response.</span></span> <span data-ttu-id="8460a-149">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="8460a-149">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8460a-150">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8460a-150">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "response", "@odata.type": "Edm.String" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json;odata.metadata=minimal;odata.streaming=true

{
"value" : "base-64 chart image string"
}
```

## <a name="usage"></a><span data-ttu-id="8460a-151">Uso</span><span class="sxs-lookup"><span data-stu-id="8460a-151">Usage</span></span>

<span data-ttu-id="8460a-152">Você pode exibir a cadeia de caracteres Base64 dentro de uma marca de imagem HTML: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="8460a-152">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="8460a-153">Para o comportamento padrão, use `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="8460a-153">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="8460a-154">Veja um exemplo de uma imagem de gráfico retornada com os parâmetros padrão.</span><span class="sxs-lookup"><span data-stu-id="8460a-154">Here is an example of a chart image returned with the default parameters.</span></span>

![A imagem de gráfico do Excel com altura e largura padrão.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="8460a-156">Se você quiser personalizar a exibição da imagem, especifique uma altura, largura e um modo de ajuste.</span><span class="sxs-lookup"><span data-stu-id="8460a-156">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="8460a-157">Esta é a aparência da imagem do gráfico quando você a recupera com esses parâmetros: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="8460a-157">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

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
