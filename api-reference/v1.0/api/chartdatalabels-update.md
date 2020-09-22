---
title: Atualizar chartdatalabels
description: Atualiza as propriedades do objeto chartdatalabels.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: eb45ef827102cea2a43435af4d7f5b7925843729
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059870"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="49375-103">Atualizar chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="49375-103">Update chartdatalabels</span></span>

<span data-ttu-id="49375-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49375-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49375-105">Atualiza as propriedades do objeto chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="49375-105">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="49375-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="49375-106">Permissions</span></span>
<span data-ttu-id="49375-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49375-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49375-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49375-109">Permission type</span></span>      | <span data-ttu-id="49375-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49375-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49375-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49375-111">Delegated (work or school account)</span></span> | <span data-ttu-id="49375-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49375-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="49375-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49375-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49375-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49375-114">Not supported.</span></span>    |
|<span data-ttu-id="49375-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49375-115">Application</span></span> | <span data-ttu-id="49375-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49375-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49375-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49375-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="49375-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="49375-118">Optional request headers</span></span>
| <span data-ttu-id="49375-119">Nome</span><span class="sxs-lookup"><span data-stu-id="49375-119">Name</span></span>       | <span data-ttu-id="49375-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="49375-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="49375-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="49375-121">Authorization</span></span>  | <span data-ttu-id="49375-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49375-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49375-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="49375-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="49375-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="49375-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49375-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49375-127">Request body</span></span>
<span data-ttu-id="49375-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="49375-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="49375-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49375-131">Property</span></span>     | <span data-ttu-id="49375-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="49375-132">Type</span></span>   |<span data-ttu-id="49375-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="49375-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49375-134">position</span><span class="sxs-lookup"><span data-stu-id="49375-134">position</span></span>|<span data-ttu-id="49375-135">string</span><span class="sxs-lookup"><span data-stu-id="49375-135">string</span></span>|<span data-ttu-id="49375-136">Valor de DataLabelPosition que representa a posição do rótulo de dados.</span><span class="sxs-lookup"><span data-stu-id="49375-136">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="49375-137">Os valores possíveis são: `None` , `Center` , `InsideEnd` , `InsideBase` , `OutsideEnd` , `Left` , `Right` , `Top` , `Bottom` , `BestFit` , `Callout` .</span><span class="sxs-lookup"><span data-stu-id="49375-137">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="49375-138">separator</span><span class="sxs-lookup"><span data-stu-id="49375-138">separator</span></span>|<span data-ttu-id="49375-139">string</span><span class="sxs-lookup"><span data-stu-id="49375-139">string</span></span>|<span data-ttu-id="49375-140">Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="49375-140">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="49375-141">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="49375-141">showBubbleSize</span></span>|<span data-ttu-id="49375-142">booliano</span><span class="sxs-lookup"><span data-stu-id="49375-142">boolean</span></span>|<span data-ttu-id="49375-143">Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="49375-143">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="49375-144">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="49375-144">showCategoryName</span></span>|<span data-ttu-id="49375-145">booliano</span><span class="sxs-lookup"><span data-stu-id="49375-145">boolean</span></span>|<span data-ttu-id="49375-146">Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="49375-146">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="49375-147">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="49375-147">showLegendKey</span></span>|<span data-ttu-id="49375-148">booliano</span><span class="sxs-lookup"><span data-stu-id="49375-148">boolean</span></span>|<span data-ttu-id="49375-149">Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="49375-149">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="49375-150">showPercentage</span><span class="sxs-lookup"><span data-stu-id="49375-150">showPercentage</span></span>|<span data-ttu-id="49375-151">booliano</span><span class="sxs-lookup"><span data-stu-id="49375-151">boolean</span></span>|<span data-ttu-id="49375-152">Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="49375-152">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="49375-153">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="49375-153">showSeriesName</span></span>|<span data-ttu-id="49375-154">booliano</span><span class="sxs-lookup"><span data-stu-id="49375-154">boolean</span></span>|<span data-ttu-id="49375-155">Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="49375-155">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="49375-156">showValue</span><span class="sxs-lookup"><span data-stu-id="49375-156">showValue</span></span>|<span data-ttu-id="49375-157">booliano</span><span class="sxs-lookup"><span data-stu-id="49375-157">boolean</span></span>|<span data-ttu-id="49375-158">Valor booliano que determina se o valor do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="49375-158">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="49375-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="49375-159">Response</span></span>

<span data-ttu-id="49375-160">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookChartDataLabels](../resources/chartdatalabels.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49375-160">If successful, this method returns a `200 OK` response code and updated [WorkbookChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="49375-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49375-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49375-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49375-162">Request</span></span>
<span data-ttu-id="49375-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49375-163">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49375-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="49375-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="49375-165">C#</span><span class="sxs-lookup"><span data-stu-id="49375-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartdatalabels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49375-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49375-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartdatalabels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49375-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49375-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartdatalabels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49375-168">Java</span><span class="sxs-lookup"><span data-stu-id="49375-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartdatalabels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="49375-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="49375-169">Response</span></span>
<span data-ttu-id="49375-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49375-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

