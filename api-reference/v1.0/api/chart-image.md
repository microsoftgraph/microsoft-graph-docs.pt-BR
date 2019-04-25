---
title: 'Chart: Image'
description: Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0f61866885f0798b9e96f80e22a636fb5f619e34
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581682"
---
# <a name="chart-image"></a><span data-ttu-id="0264e-103">Chart: Image</span><span class="sxs-lookup"><span data-stu-id="0264e-103">Chart: Image</span></span>

<span data-ttu-id="0264e-104">Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.</span><span class="sxs-lookup"><span data-stu-id="0264e-104">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="0264e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0264e-105">Permissions</span></span>
<span data-ttu-id="0264e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0264e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0264e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0264e-108">Permission type</span></span>      | <span data-ttu-id="0264e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0264e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0264e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0264e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0264e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0264e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0264e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0264e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0264e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0264e-113">Not supported.</span></span>    |
|<span data-ttu-id="0264e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0264e-114">Application</span></span> | <span data-ttu-id="0264e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0264e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0264e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0264e-116">HTTP request</span></span>
<!-- { "blockType": "samples" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/image
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```
## <a name="request-headers"></a><span data-ttu-id="0264e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0264e-117">Request headers</span></span>
| <span data-ttu-id="0264e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0264e-118">Name</span></span>       | <span data-ttu-id="0264e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0264e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0264e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0264e-120">Authorization</span></span>  | <span data-ttu-id="0264e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0264e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0264e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0264e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0264e-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0264e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="0264e-126">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="0264e-126">Path parameters</span></span>
<span data-ttu-id="0264e-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0264e-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0264e-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0264e-128">Parameter</span></span>    | <span data-ttu-id="0264e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0264e-129">Type</span></span>   |<span data-ttu-id="0264e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0264e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0264e-131">height</span><span class="sxs-lookup"><span data-stu-id="0264e-131">height</span></span>|<span data-ttu-id="0264e-132">Int32</span><span class="sxs-lookup"><span data-stu-id="0264e-132">Int32</span></span>|<span data-ttu-id="0264e-133">A altura desejada da imagem resultante.</span><span class="sxs-lookup"><span data-stu-id="0264e-133">The desired height of the resulting image.</span></span> <span data-ttu-id="0264e-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0264e-134">Optional.</span></span>|
|<span data-ttu-id="0264e-135">width</span><span class="sxs-lookup"><span data-stu-id="0264e-135">width</span></span>|<span data-ttu-id="0264e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="0264e-136">Int32</span></span>|<span data-ttu-id="0264e-137">A largura desejada da imagem resultante.</span><span class="sxs-lookup"><span data-stu-id="0264e-137">The desired width of the resulting image.</span></span> <span data-ttu-id="0264e-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0264e-138">Optional.</span></span>|
|<span data-ttu-id="0264e-139">fittingMode</span><span class="sxs-lookup"><span data-stu-id="0264e-139">fittingMode</span></span>|<span data-ttu-id="0264e-140">string</span><span class="sxs-lookup"><span data-stu-id="0264e-140">string</span></span>|<span data-ttu-id="0264e-141">O método usado para dimensionar o gráfico para as dimensões especificadas (se a altura e a largura forem definidas). "</span><span class="sxs-lookup"><span data-stu-id="0264e-141">The method used to scale the chart to the specified dimensions (if both height and width are set)."</span></span>  <span data-ttu-id="0264e-142">Os valores possíveis são: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="0264e-142">The possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="0264e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="0264e-143">Response</span></span>

<span data-ttu-id="0264e-144">Se bem-sucedido, este método retorna o código de resposta `200 OK` e a cadeia de caracteres de imagem em base64 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0264e-144">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0264e-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0264e-145">Example</span></span>
<span data-ttu-id="0264e-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0264e-146">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="0264e-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0264e-147">Request</span></span>
<span data-ttu-id="0264e-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0264e-148">Here is an example of the request.</span></span>

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="0264e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="0264e-149">Response</span></span>
<span data-ttu-id="0264e-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0264e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "response", "@odata.type": "Edm.String" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json;odata.metadata=minimal;odata.streaming=true

{
"value" : "base-64 chart image string"
}
```

## <a name="usage"></a><span data-ttu-id="0264e-153">Uso</span><span class="sxs-lookup"><span data-stu-id="0264e-153">Usage</span></span>

<span data-ttu-id="0264e-154">Você pode exibir a cadeia de caracteres Base64 dentro de uma marca de imagem HTML: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="0264e-154">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="0264e-155">Para o comportamento padrão, use `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="0264e-155">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="0264e-156">Veja um exemplo de uma imagem de gráfico retornada com os parâmetros padrão.</span><span class="sxs-lookup"><span data-stu-id="0264e-156">Here is an example of a chart image returned with the default parameters.</span></span>

![A imagem de gráfico do Excel com altura e largura padrão.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="0264e-158">Se você quiser personalizar a exibição da imagem, especifique uma altura, largura e um modo de ajuste.</span><span class="sxs-lookup"><span data-stu-id="0264e-158">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="0264e-159">Esta é a aparência da imagem do gráfico quando você a recupera com esses parâmetros: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="0264e-159">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

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
