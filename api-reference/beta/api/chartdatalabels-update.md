---
title: Atualizar chartdatalabels
description: Atualiza as propriedades do objeto chartdatalabels.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b7eb067bed747ae2532939e61a9e0dec58ff4655
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518293"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="bd5c6-103">Atualizar chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="bd5c6-103">Update chartdatalabels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd5c6-104">Atualiza as propriedades do objeto chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="bd5c6-104">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bd5c6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd5c6-105">Permissions</span></span>
<span data-ttu-id="bd5c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd5c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd5c6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd5c6-108">Permission type</span></span>      | <span data-ttu-id="bd5c6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd5c6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd5c6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd5c6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bd5c6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd5c6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bd5c6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd5c6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd5c6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd5c6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bd5c6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd5c6-114">Application</span></span> | <span data-ttu-id="bd5c6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd5c6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd5c6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd5c6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="bd5c6-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="bd5c6-117">Optional request headers</span></span>
| <span data-ttu-id="bd5c6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bd5c6-118">Name</span></span>       | <span data-ttu-id="bd5c6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd5c6-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bd5c6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd5c6-120">Authorization</span></span>  | <span data-ttu-id="bd5c6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd5c6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bd5c6-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bd5c6-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bd5c6-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="bd5c6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd5c6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd5c6-126">Request body</span></span>
<span data-ttu-id="bd5c6-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bd5c6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bd5c6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd5c6-130">Property</span></span>     | <span data-ttu-id="bd5c6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd5c6-131">Type</span></span>   |<span data-ttu-id="bd5c6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd5c6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd5c6-133">position</span><span class="sxs-lookup"><span data-stu-id="bd5c6-133">position</span></span>|<span data-ttu-id="bd5c6-134">string</span><span class="sxs-lookup"><span data-stu-id="bd5c6-134">string</span></span>|<span data-ttu-id="bd5c6-p105">Valor de DataLabelPosition que representa a posição do rótulo de dados. Os valores possíveis são: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit` e `Callout`.</span><span class="sxs-lookup"><span data-stu-id="bd5c6-p105">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="bd5c6-137">separador</span><span class="sxs-lookup"><span data-stu-id="bd5c6-137">separator</span></span>|<span data-ttu-id="bd5c6-138">string</span><span class="sxs-lookup"><span data-stu-id="bd5c6-138">string</span></span>|<span data-ttu-id="bd5c6-139">Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="bd5c6-139">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="bd5c6-140">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="bd5c6-140">showBubbleSize</span></span>|<span data-ttu-id="bd5c6-141">booliano</span><span class="sxs-lookup"><span data-stu-id="bd5c6-141">boolean</span></span>|<span data-ttu-id="bd5c6-142">Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="bd5c6-142">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="bd5c6-143">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="bd5c6-143">showCategoryName</span></span>|<span data-ttu-id="bd5c6-144">booliano</span><span class="sxs-lookup"><span data-stu-id="bd5c6-144">boolean</span></span>|<span data-ttu-id="bd5c6-145">Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="bd5c6-145">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="bd5c6-146">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="bd5c6-146">showLegendKey</span></span>|<span data-ttu-id="bd5c6-147">booliano</span><span class="sxs-lookup"><span data-stu-id="bd5c6-147">boolean</span></span>|<span data-ttu-id="bd5c6-148">Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="bd5c6-148">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="bd5c6-149">showPercentage</span><span class="sxs-lookup"><span data-stu-id="bd5c6-149">showPercentage</span></span>|<span data-ttu-id="bd5c6-150">booliano</span><span class="sxs-lookup"><span data-stu-id="bd5c6-150">boolean</span></span>|<span data-ttu-id="bd5c6-151">Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="bd5c6-151">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="bd5c6-152">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="bd5c6-152">showSeriesName</span></span>|<span data-ttu-id="bd5c6-153">booliano</span><span class="sxs-lookup"><span data-stu-id="bd5c6-153">boolean</span></span>|<span data-ttu-id="bd5c6-154">Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="bd5c6-154">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="bd5c6-155">showValue</span><span class="sxs-lookup"><span data-stu-id="bd5c6-155">showValue</span></span>|<span data-ttu-id="bd5c6-156">booliano</span><span class="sxs-lookup"><span data-stu-id="bd5c6-156">boolean</span></span>|<span data-ttu-id="bd5c6-157">Valor booliano que determina se o valor do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="bd5c6-157">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="bd5c6-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd5c6-158">Response</span></span>

<span data-ttu-id="bd5c6-159">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartDataLabels](../resources/chartdatalabels.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd5c6-159">If successful, this method returns a `200 OK` response code and updated [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bd5c6-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd5c6-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd5c6-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd5c6-161">Request</span></span>
<span data-ttu-id="bd5c6-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd5c6-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/datalabels
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
##### <a name="response"></a><span data-ttu-id="bd5c6-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd5c6-163">Response</span></span>
<span data-ttu-id="bd5c6-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd5c6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartDataLabels"
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
    "Error: /api-reference/beta/api/chartdatalabels-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
