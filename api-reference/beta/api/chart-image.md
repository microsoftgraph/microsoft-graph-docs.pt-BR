---
title: 'Chart: Image'
description: Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5ee56b38ca75162a760be54e58dacb6ced6bbc16
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976405"
---
# <a name="chart-image"></a><span data-ttu-id="304bb-103">Chart: Image</span><span class="sxs-lookup"><span data-stu-id="304bb-103">Chart: Image</span></span>

> <span data-ttu-id="304bb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="304bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="304bb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="304bb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="304bb-106">Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.</span><span class="sxs-lookup"><span data-stu-id="304bb-106">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="304bb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="304bb-107">Permissions</span></span>
<span data-ttu-id="304bb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="304bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="304bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="304bb-110">Permission type</span></span>      | <span data-ttu-id="304bb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="304bb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="304bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="304bb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="304bb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="304bb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="304bb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="304bb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="304bb-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="304bb-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="304bb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="304bb-116">Application</span></span> | <span data-ttu-id="304bb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="304bb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="304bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="304bb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="304bb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="304bb-119">Request headers</span></span>
| <span data-ttu-id="304bb-120">Nome</span><span class="sxs-lookup"><span data-stu-id="304bb-120">Name</span></span>       | <span data-ttu-id="304bb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="304bb-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="304bb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="304bb-122">Authorization</span></span>  | <span data-ttu-id="304bb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="304bb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="304bb-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="304bb-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="304bb-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="304bb-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="304bb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="304bb-128">Request body</span></span>
<span data-ttu-id="304bb-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="304bb-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="304bb-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="304bb-130">Parameter</span></span>    | <span data-ttu-id="304bb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="304bb-131">Type</span></span>   |<span data-ttu-id="304bb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="304bb-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="304bb-133">height</span><span class="sxs-lookup"><span data-stu-id="304bb-133">height</span></span>|<span data-ttu-id="304bb-134">number</span><span class="sxs-lookup"><span data-stu-id="304bb-134">number</span></span>|<span data-ttu-id="304bb-p105">Opcional. A altura desejada da imagem resultante.</span><span class="sxs-lookup"><span data-stu-id="304bb-p105">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="304bb-137">width</span><span class="sxs-lookup"><span data-stu-id="304bb-137">width</span></span>|<span data-ttu-id="304bb-138">number</span><span class="sxs-lookup"><span data-stu-id="304bb-138">number</span></span>|<span data-ttu-id="304bb-p106">Opcional. A largura desejada da imagem resultante.</span><span class="sxs-lookup"><span data-stu-id="304bb-p106">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="304bb-141">fittingMode</span><span class="sxs-lookup"><span data-stu-id="304bb-141">fittingMode</span></span>|<span data-ttu-id="304bb-142">string</span><span class="sxs-lookup"><span data-stu-id="304bb-142">string</span></span>|<span data-ttu-id="304bb-p107">Opcional. O método usado para dimensionar o gráfico para as dimensões especificadas (se height e width tiverem sido definidas).  Os valores possíveis são: `Fit`, `FitAndCenter` e `Fill`.</span><span class="sxs-lookup"><span data-stu-id="304bb-p107">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="304bb-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="304bb-146">Response</span></span>

<span data-ttu-id="304bb-147">Se bem-sucedido, este método retorna o código de resposta `200 OK` e a cadeia de caracteres de imagem em base64 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="304bb-147">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="304bb-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="304bb-148">Example</span></span>
<span data-ttu-id="304bb-149">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="304bb-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="304bb-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="304bb-150">Request</span></span>
<span data-ttu-id="304bb-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="304bb-151">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="304bb-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="304bb-152">Response</span></span>
<span data-ttu-id="304bb-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="304bb-153">Here is an example of the response.</span></span> <span data-ttu-id="304bb-154">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="304bb-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="304bb-155">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="304bb-155">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

##### <a name="usage"></a><span data-ttu-id="304bb-156">Uso</span><span class="sxs-lookup"><span data-stu-id="304bb-156">Usage</span></span>

<span data-ttu-id="304bb-157">Você pode exibir a cadeia de caracteres Base64 dentro de uma marca de imagem HTML: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="304bb-157">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="304bb-158">Para o comportamento padrão, use `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="304bb-158">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="304bb-159">Veja um exemplo de uma imagem de gráfico retornada com os parâmetros padrão.</span><span class="sxs-lookup"><span data-stu-id="304bb-159">Here is an example of a chart image returned with the default parameters.</span></span>

![A imagem de gráfico do Excel com altura e largura padrão.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="304bb-161">Se você quiser personalizar a exibição da imagem, especifique uma altura, largura e um modo de ajuste.</span><span class="sxs-lookup"><span data-stu-id="304bb-161">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="304bb-162">Esta é a aparência da imagem do gráfico quando você a recupera com esses parâmetros: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="304bb-162">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

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
