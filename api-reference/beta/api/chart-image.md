---
title: 'Chart: Image'
description: Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 997948cbae8b8df135c01da20bf3b508c95eed97
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047515"
---
# <a name="chart-image"></a><span data-ttu-id="fa22c-103">Chart: Image</span><span class="sxs-lookup"><span data-stu-id="fa22c-103">Chart: Image</span></span>

<span data-ttu-id="fa22c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa22c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa22c-105">Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.</span><span class="sxs-lookup"><span data-stu-id="fa22c-105">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="fa22c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa22c-106">Permissions</span></span>
<span data-ttu-id="fa22c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa22c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa22c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa22c-109">Permission type</span></span>      | <span data-ttu-id="fa22c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa22c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa22c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa22c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fa22c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa22c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fa22c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa22c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa22c-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa22c-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fa22c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa22c-115">Application</span></span> | <span data-ttu-id="fa22c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa22c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa22c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa22c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/Image(width=0,height=0,fittingMode='fit')
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="fa22c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa22c-118">Request headers</span></span>
| <span data-ttu-id="fa22c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fa22c-119">Name</span></span>       | <span data-ttu-id="fa22c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa22c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fa22c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa22c-121">Authorization</span></span>  | <span data-ttu-id="fa22c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa22c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa22c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fa22c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="fa22c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="fa22c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa22c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa22c-127">Request body</span></span>
<span data-ttu-id="fa22c-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa22c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fa22c-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fa22c-129">Parameter</span></span>    | <span data-ttu-id="fa22c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa22c-130">Type</span></span>   |<span data-ttu-id="fa22c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa22c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa22c-132">height</span><span class="sxs-lookup"><span data-stu-id="fa22c-132">height</span></span>|<span data-ttu-id="fa22c-133">number</span><span class="sxs-lookup"><span data-stu-id="fa22c-133">number</span></span>|<span data-ttu-id="fa22c-p104">Opcional. A altura desejada da imagem resultante.</span><span class="sxs-lookup"><span data-stu-id="fa22c-p104">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="fa22c-136">width</span><span class="sxs-lookup"><span data-stu-id="fa22c-136">width</span></span>|<span data-ttu-id="fa22c-137">number</span><span class="sxs-lookup"><span data-stu-id="fa22c-137">number</span></span>|<span data-ttu-id="fa22c-p105">Opcional. A largura desejada da imagem resultante.</span><span class="sxs-lookup"><span data-stu-id="fa22c-p105">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="fa22c-140">fittingMode</span><span class="sxs-lookup"><span data-stu-id="fa22c-140">fittingMode</span></span>|<span data-ttu-id="fa22c-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa22c-141">string</span></span>|<span data-ttu-id="fa22c-p106">Opcional. O método usado para dimensionar o gráfico para as dimensões especificadas (se height e width tiverem sido definidas).  Os valores possíveis são: `Fit`, `FitAndCenter` e `Fill`.</span><span class="sxs-lookup"><span data-stu-id="fa22c-p106">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="fa22c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa22c-145">Response</span></span>

<span data-ttu-id="fa22c-146">Se bem-sucedido, este método retorna o código de resposta `200 OK` e a cadeia de caracteres de imagem em base64 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa22c-146">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa22c-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa22c-147">Example</span></span>
<span data-ttu-id="fa22c-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fa22c-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fa22c-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa22c-149">Request</span></span>
<span data-ttu-id="fa22c-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa22c-150">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="fa22c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa22c-151">Response</span></span>
<span data-ttu-id="fa22c-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa22c-152">Here is an example of the response.</span></span> <span data-ttu-id="fa22c-153">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fa22c-153">Note: The response object shown here might be shortened for readability.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

##### <a name="usage"></a><span data-ttu-id="fa22c-154">Uso</span><span class="sxs-lookup"><span data-stu-id="fa22c-154">Usage</span></span>

<span data-ttu-id="fa22c-155">Você pode exibir a cadeia de caracteres de Base 64 dentro de uma marca de imagem HTML: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="fa22c-155">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="fa22c-156">Para o comportamento padrão, use `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="fa22c-156">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="fa22c-157">Veja um exemplo de uma imagem de gráfico retornada com os parâmetros padrão.</span><span class="sxs-lookup"><span data-stu-id="fa22c-157">Here is an example of a chart image returned with the default parameters.</span></span>

![A imagem de gráfico do Excel com altura e largura padrão.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="fa22c-159">Se você quiser personalizar a exibição da imagem, especifique uma altura, largura e um modo de ajuste.</span><span class="sxs-lookup"><span data-stu-id="fa22c-159">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="fa22c-160">Esta é a aparência da imagem de gráfico quando você a recupera com esses parâmetros: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="fa22c-160">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

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
  "suppressions": []
}
-->


