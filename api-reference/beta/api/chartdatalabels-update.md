---
title: Atualizar workbookChartDataLabels
description: Atualize as propriedades do objeto workbookchartdatalabels.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c8eea755c543f3373ac157551824c47d8d82d13e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418492"
---
# <a name="update-workbookchartdatalabels"></a><span data-ttu-id="c88b7-103">Atualizar workbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="c88b7-103">Update workbookChartDataLabels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c88b7-104">Atualiza as propriedades do objeto chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="c88b7-104">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c88b7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c88b7-105">Permissions</span></span>
<span data-ttu-id="c88b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c88b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c88b7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c88b7-108">Permission type</span></span>      | <span data-ttu-id="c88b7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c88b7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c88b7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c88b7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c88b7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c88b7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c88b7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c88b7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c88b7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c88b7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c88b7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c88b7-114">Application</span></span> | <span data-ttu-id="c88b7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c88b7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c88b7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c88b7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="c88b7-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c88b7-117">Optional request headers</span></span>
| <span data-ttu-id="c88b7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c88b7-118">Name</span></span>       | <span data-ttu-id="c88b7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c88b7-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c88b7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c88b7-120">Authorization</span></span>  | <span data-ttu-id="c88b7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c88b7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c88b7-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c88b7-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c88b7-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c88b7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c88b7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c88b7-126">Request body</span></span>
<span data-ttu-id="c88b7-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c88b7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c88b7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c88b7-130">Property</span></span>     | <span data-ttu-id="c88b7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c88b7-131">Type</span></span>   |<span data-ttu-id="c88b7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c88b7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c88b7-133">position</span><span class="sxs-lookup"><span data-stu-id="c88b7-133">position</span></span>|<span data-ttu-id="c88b7-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c88b7-134">string</span></span>|<span data-ttu-id="c88b7-p105">Valor de DataLabelPosition que representa a posição do rótulo de dados. Os valores possíveis são: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit` e `Callout`.</span><span class="sxs-lookup"><span data-stu-id="c88b7-p105">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="c88b7-137">separador</span><span class="sxs-lookup"><span data-stu-id="c88b7-137">separator</span></span>|<span data-ttu-id="c88b7-138">string</span><span class="sxs-lookup"><span data-stu-id="c88b7-138">string</span></span>|<span data-ttu-id="c88b7-139">Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="c88b7-139">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="c88b7-140">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="c88b7-140">showBubbleSize</span></span>|<span data-ttu-id="c88b7-141">booliano</span><span class="sxs-lookup"><span data-stu-id="c88b7-141">boolean</span></span>|<span data-ttu-id="c88b7-142">Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="c88b7-142">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="c88b7-143">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="c88b7-143">showCategoryName</span></span>|<span data-ttu-id="c88b7-144">booliano</span><span class="sxs-lookup"><span data-stu-id="c88b7-144">boolean</span></span>|<span data-ttu-id="c88b7-145">Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="c88b7-145">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="c88b7-146">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="c88b7-146">showLegendKey</span></span>|<span data-ttu-id="c88b7-147">booliano</span><span class="sxs-lookup"><span data-stu-id="c88b7-147">boolean</span></span>|<span data-ttu-id="c88b7-148">Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="c88b7-148">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="c88b7-149">showPercentage</span><span class="sxs-lookup"><span data-stu-id="c88b7-149">showPercentage</span></span>|<span data-ttu-id="c88b7-150">booliano</span><span class="sxs-lookup"><span data-stu-id="c88b7-150">boolean</span></span>|<span data-ttu-id="c88b7-151">Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="c88b7-151">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="c88b7-152">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="c88b7-152">showSeriesName</span></span>|<span data-ttu-id="c88b7-153">booliano</span><span class="sxs-lookup"><span data-stu-id="c88b7-153">boolean</span></span>|<span data-ttu-id="c88b7-154">Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="c88b7-154">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="c88b7-155">showValue</span><span class="sxs-lookup"><span data-stu-id="c88b7-155">showValue</span></span>|<span data-ttu-id="c88b7-156">booliano</span><span class="sxs-lookup"><span data-stu-id="c88b7-156">boolean</span></span>|<span data-ttu-id="c88b7-157">Valor booliano que determina se o valor do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="c88b7-157">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="c88b7-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="c88b7-158">Response</span></span>

<span data-ttu-id="c88b7-159">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookChartDataLabels](../resources/workbookchartdatalabels.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c88b7-159">If successful, this method returns a `200 OK` response code and updated [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c88b7-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c88b7-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c88b7-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c88b7-161">Request</span></span>
<span data-ttu-id="c88b7-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c88b7-162">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c88b7-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="c88b7-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/datalabels
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c88b7-164">C#</span><span class="sxs-lookup"><span data-stu-id="c88b7-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartdatalabels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c88b7-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c88b7-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartdatalabels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c88b7-166">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c88b7-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartdatalabels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c88b7-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="c88b7-167">Response</span></span>
<span data-ttu-id="c88b7-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c88b7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
