---
title: 'Chart: Image'
description: Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b354be83058d67dc99cd3ffd7c98798017733199
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518571"
---
# <a name="chart-image"></a><span data-ttu-id="20765-103">Chart: Image</span><span class="sxs-lookup"><span data-stu-id="20765-103">Chart: Image</span></span>

<span data-ttu-id="20765-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20765-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="20765-105">Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.</span><span class="sxs-lookup"><span data-stu-id="20765-105">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="20765-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="20765-106">Permissions</span></span>
<span data-ttu-id="20765-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20765-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20765-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20765-109">Permission type</span></span>      | <span data-ttu-id="20765-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20765-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20765-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20765-111">Delegated (work or school account)</span></span> | <span data-ttu-id="20765-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20765-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="20765-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20765-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20765-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20765-114">Not supported.</span></span>    |
|<span data-ttu-id="20765-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20765-115">Application</span></span> | <span data-ttu-id="20765-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20765-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20765-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20765-117">HTTP request</span></span>
<!-- { "blockType": "samples" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/image
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```
## <a name="request-headers"></a><span data-ttu-id="20765-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20765-118">Request headers</span></span>
| <span data-ttu-id="20765-119">Nome</span><span class="sxs-lookup"><span data-stu-id="20765-119">Name</span></span>       | <span data-ttu-id="20765-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="20765-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="20765-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="20765-121">Authorization</span></span>  | <span data-ttu-id="20765-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20765-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20765-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="20765-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="20765-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="20765-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="20765-127">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="20765-127">Path parameters</span></span>
<span data-ttu-id="20765-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20765-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="20765-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="20765-129">Parameter</span></span>    | <span data-ttu-id="20765-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="20765-130">Type</span></span>   |<span data-ttu-id="20765-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="20765-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20765-132">height</span><span class="sxs-lookup"><span data-stu-id="20765-132">height</span></span>|<span data-ttu-id="20765-133">Int32</span><span class="sxs-lookup"><span data-stu-id="20765-133">Int32</span></span>|<span data-ttu-id="20765-134">A altura desejada da imagem resultante.</span><span class="sxs-lookup"><span data-stu-id="20765-134">The desired height of the resulting image.</span></span> <span data-ttu-id="20765-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="20765-135">Optional.</span></span>|
|<span data-ttu-id="20765-136">width</span><span class="sxs-lookup"><span data-stu-id="20765-136">width</span></span>|<span data-ttu-id="20765-137">Int32</span><span class="sxs-lookup"><span data-stu-id="20765-137">Int32</span></span>|<span data-ttu-id="20765-138">A largura desejada da imagem resultante.</span><span class="sxs-lookup"><span data-stu-id="20765-138">The desired width of the resulting image.</span></span> <span data-ttu-id="20765-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="20765-139">Optional.</span></span>|
|<span data-ttu-id="20765-140">fittingMode</span><span class="sxs-lookup"><span data-stu-id="20765-140">fittingMode</span></span>|<span data-ttu-id="20765-141">string</span><span class="sxs-lookup"><span data-stu-id="20765-141">string</span></span>|<span data-ttu-id="20765-142">O método usado para dimensionar o gráfico para as dimensões especificadas (se a altura e a largura forem definidas). "</span><span class="sxs-lookup"><span data-stu-id="20765-142">The method used to scale the chart to the specified dimensions (if both height and width are set)."</span></span>  <span data-ttu-id="20765-143">Os valores possíveis são: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="20765-143">The possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="20765-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="20765-144">Response</span></span>

<span data-ttu-id="20765-145">Se bem-sucedido, este método retorna o código de resposta `200 OK` e a cadeia de caracteres de imagem em base64 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20765-145">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20765-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20765-146">Example</span></span>
<span data-ttu-id="20765-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="20765-147">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="20765-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20765-148">Request</span></span>
<span data-ttu-id="20765-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20765-149">Here is an example of the request.</span></span>

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="20765-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="20765-150">Response</span></span>
<span data-ttu-id="20765-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20765-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "response", "@odata.type": "Edm.String" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json;odata.metadata=minimal;odata.streaming=true

{
"value" : "base-64 chart image string"
}
```

## <a name="usage"></a><span data-ttu-id="20765-154">Uso</span><span class="sxs-lookup"><span data-stu-id="20765-154">Usage</span></span>

<span data-ttu-id="20765-155">Você pode exibir a cadeia de caracteres de Base 64 dentro de uma marca de imagem HTML: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="20765-155">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="20765-156">Para o comportamento padrão, use `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="20765-156">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="20765-157">Veja um exemplo de uma imagem de gráfico retornada com os parâmetros padrão.</span><span class="sxs-lookup"><span data-stu-id="20765-157">Here is an example of a chart image returned with the default parameters.</span></span>

![A imagem de gráfico do Excel com altura e largura padrão.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="20765-159">Se você quiser personalizar a exibição da imagem, especifique uma altura, largura e um modo de ajuste.</span><span class="sxs-lookup"><span data-stu-id="20765-159">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="20765-160">Esta é a aparência da imagem de gráfico quando você a recupera com esses parâmetros: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="20765-160">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

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
