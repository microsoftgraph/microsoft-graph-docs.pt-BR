---
title: 'Chart: Image'
description: Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5892864d8adb94c4c6193dc4776f8febd938ff36
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642839"
---
# <a name="chart-image"></a><span data-ttu-id="34bf9-103">Chart: Image</span><span class="sxs-lookup"><span data-stu-id="34bf9-103">Chart: Image</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34bf9-104">Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.</span><span class="sxs-lookup"><span data-stu-id="34bf9-104">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="34bf9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="34bf9-105">Permissions</span></span>
<span data-ttu-id="34bf9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34bf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34bf9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34bf9-108">Permission type</span></span>      | <span data-ttu-id="34bf9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34bf9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34bf9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34bf9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="34bf9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34bf9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34bf9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34bf9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34bf9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34bf9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34bf9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34bf9-114">Application</span></span> | <span data-ttu-id="34bf9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34bf9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34bf9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34bf9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="34bf9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34bf9-117">Request headers</span></span>
| <span data-ttu-id="34bf9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="34bf9-118">Name</span></span>       | <span data-ttu-id="34bf9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="34bf9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="34bf9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="34bf9-120">Authorization</span></span>  | <span data-ttu-id="34bf9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34bf9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34bf9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="34bf9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="34bf9-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="34bf9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34bf9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34bf9-126">Request body</span></span>
<span data-ttu-id="34bf9-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34bf9-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="34bf9-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="34bf9-128">Parameter</span></span>    | <span data-ttu-id="34bf9-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="34bf9-129">Type</span></span>   |<span data-ttu-id="34bf9-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="34bf9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34bf9-131">height</span><span class="sxs-lookup"><span data-stu-id="34bf9-131">height</span></span>|<span data-ttu-id="34bf9-132">number</span><span class="sxs-lookup"><span data-stu-id="34bf9-132">number</span></span>|<span data-ttu-id="34bf9-p104">Opcional. A altura desejada da imagem resultante.</span><span class="sxs-lookup"><span data-stu-id="34bf9-p104">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="34bf9-135">width</span><span class="sxs-lookup"><span data-stu-id="34bf9-135">width</span></span>|<span data-ttu-id="34bf9-136">number</span><span class="sxs-lookup"><span data-stu-id="34bf9-136">number</span></span>|<span data-ttu-id="34bf9-p105">Opcional. A largura desejada da imagem resultante.</span><span class="sxs-lookup"><span data-stu-id="34bf9-p105">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="34bf9-139">fittingMode</span><span class="sxs-lookup"><span data-stu-id="34bf9-139">fittingMode</span></span>|<span data-ttu-id="34bf9-140">string</span><span class="sxs-lookup"><span data-stu-id="34bf9-140">string</span></span>|<span data-ttu-id="34bf9-p106">Opcional. O método usado para dimensionar o gráfico para as dimensões especificadas (se height e width tiverem sido definidas).  Os valores possíveis são: `Fit`, `FitAndCenter` e `Fill`.</span><span class="sxs-lookup"><span data-stu-id="34bf9-p106">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="34bf9-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="34bf9-144">Response</span></span>

<span data-ttu-id="34bf9-145">Se bem-sucedido, este método retorna o código de resposta `200 OK` e a cadeia de caracteres de imagem em base64 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34bf9-145">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34bf9-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34bf9-146">Example</span></span>
<span data-ttu-id="34bf9-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="34bf9-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="34bf9-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34bf9-148">Request</span></span>
<span data-ttu-id="34bf9-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34bf9-149">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="34bf9-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="34bf9-150">Response</span></span>
<span data-ttu-id="34bf9-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34bf9-151">Here is an example of the response.</span></span> <span data-ttu-id="34bf9-152">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="34bf9-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="34bf9-153">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34bf9-153">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

##### <a name="usage"></a><span data-ttu-id="34bf9-154">Uso</span><span class="sxs-lookup"><span data-stu-id="34bf9-154">Usage</span></span>

<span data-ttu-id="34bf9-155">Você pode exibir a cadeia de caracteres Base64 dentro de uma marca de imagem HTML: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="34bf9-155">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="34bf9-156">Para o comportamento padrão, use `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="34bf9-156">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="34bf9-157">Veja um exemplo de uma imagem de gráfico retornada com os parâmetros padrão.</span><span class="sxs-lookup"><span data-stu-id="34bf9-157">Here is an example of a chart image returned with the default parameters.</span></span>

![A imagem de gráfico do Excel com altura e largura padrão.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="34bf9-159">Se você quiser personalizar a exibição da imagem, especifique uma altura, largura e um modo de ajuste.</span><span class="sxs-lookup"><span data-stu-id="34bf9-159">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="34bf9-160">Esta é a aparência da imagem do gráfico quando você a recupera com esses parâmetros: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="34bf9-160">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

![A imagem de gráfico do Excel com altura e largura padrão.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-fill.png)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-image.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
