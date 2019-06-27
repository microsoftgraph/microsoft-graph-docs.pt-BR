---
title: Atualizar chartdatalabels
description: Atualiza as propriedades do objeto chartdatalabels.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4ad66f2cbf4d78c1fd3570d9e98184370b0ef075
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272517"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="0a3f7-103">Atualizar chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="0a3f7-103">Update chartdatalabels</span></span>

<span data-ttu-id="0a3f7-104">Atualiza as propriedades do objeto chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-104">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0a3f7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0a3f7-105">Permissions</span></span>
<span data-ttu-id="0a3f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a3f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a3f7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a3f7-108">Permission type</span></span>      | <span data-ttu-id="0a3f7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a3f7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a3f7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a3f7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0a3f7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a3f7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0a3f7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a3f7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a3f7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-113">Not supported.</span></span>    |
|<span data-ttu-id="0a3f7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a3f7-114">Application</span></span> | <span data-ttu-id="0a3f7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a3f7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a3f7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="0a3f7-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="0a3f7-117">Optional request headers</span></span>
| <span data-ttu-id="0a3f7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0a3f7-118">Name</span></span>       | <span data-ttu-id="0a3f7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a3f7-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0a3f7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a3f7-120">Authorization</span></span>  | <span data-ttu-id="0a3f7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0a3f7-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0a3f7-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0a3f7-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a3f7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a3f7-126">Request body</span></span>
<span data-ttu-id="0a3f7-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0a3f7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a3f7-130">Property</span></span>     | <span data-ttu-id="0a3f7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a3f7-131">Type</span></span>   |<span data-ttu-id="0a3f7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a3f7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a3f7-133">position</span><span class="sxs-lookup"><span data-stu-id="0a3f7-133">position</span></span>|<span data-ttu-id="0a3f7-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a3f7-134">string</span></span>|<span data-ttu-id="0a3f7-135">Valor de DataLabelPosition que representa a posição do rótulo de dados.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-135">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="0a3f7-136">Os valores possíveis são: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-136">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="0a3f7-137">separator</span><span class="sxs-lookup"><span data-stu-id="0a3f7-137">separator</span></span>|<span data-ttu-id="0a3f7-138">string</span><span class="sxs-lookup"><span data-stu-id="0a3f7-138">string</span></span>|<span data-ttu-id="0a3f7-139">Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-139">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="0a3f7-140">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="0a3f7-140">showBubbleSize</span></span>|<span data-ttu-id="0a3f7-141">booliano</span><span class="sxs-lookup"><span data-stu-id="0a3f7-141">boolean</span></span>|<span data-ttu-id="0a3f7-142">Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-142">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="0a3f7-143">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="0a3f7-143">showCategoryName</span></span>|<span data-ttu-id="0a3f7-144">booliano</span><span class="sxs-lookup"><span data-stu-id="0a3f7-144">boolean</span></span>|<span data-ttu-id="0a3f7-145">Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-145">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="0a3f7-146">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="0a3f7-146">showLegendKey</span></span>|<span data-ttu-id="0a3f7-147">booliano</span><span class="sxs-lookup"><span data-stu-id="0a3f7-147">boolean</span></span>|<span data-ttu-id="0a3f7-148">Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-148">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="0a3f7-149">showPercentage</span><span class="sxs-lookup"><span data-stu-id="0a3f7-149">showPercentage</span></span>|<span data-ttu-id="0a3f7-150">booliano</span><span class="sxs-lookup"><span data-stu-id="0a3f7-150">boolean</span></span>|<span data-ttu-id="0a3f7-151">Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-151">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="0a3f7-152">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="0a3f7-152">showSeriesName</span></span>|<span data-ttu-id="0a3f7-153">booliano</span><span class="sxs-lookup"><span data-stu-id="0a3f7-153">boolean</span></span>|<span data-ttu-id="0a3f7-154">Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-154">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="0a3f7-155">showValue</span><span class="sxs-lookup"><span data-stu-id="0a3f7-155">showValue</span></span>|<span data-ttu-id="0a3f7-156">booliano</span><span class="sxs-lookup"><span data-stu-id="0a3f7-156">boolean</span></span>|<span data-ttu-id="0a3f7-157">Valor booliano que determina se o valor do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-157">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="0a3f7-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a3f7-158">Response</span></span>

<span data-ttu-id="0a3f7-159">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookChartDataLabels](../resources/chartdatalabels.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-159">If successful, this method returns a `200 OK` response code and updated [WorkbookChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0a3f7-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a3f7-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a3f7-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a3f7-161">Request</span></span>
<span data-ttu-id="0a3f7-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels
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
##### <a name="response"></a><span data-ttu-id="0a3f7-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a3f7-163">Response</span></span>
<span data-ttu-id="0a3f7-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a3f7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0a3f7-167">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="0a3f7-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0a3f7-168">C#</span><span class="sxs-lookup"><span data-stu-id="0a3f7-168">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_chartdatalabels-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a3f7-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="0a3f7-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_chartdatalabels-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0a3f7-170">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0a3f7-170">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_chartdatalabels-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/chartdatalabels-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/chartdatalabels-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/chartdatalabels-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
