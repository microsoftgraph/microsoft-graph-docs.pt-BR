---
title: Atualizar chartdatalabels
description: Atualiza as propriedades do objeto chartdatalabels.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f61113f8cd0617d6d8eb3f3191112d74e55f27cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985433"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="ebaf7-103">Atualizar chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="ebaf7-103">Update chartdatalabels</span></span>

> <span data-ttu-id="ebaf7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebaf7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ebaf7-106">Atualiza as propriedades do objeto chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-106">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ebaf7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ebaf7-107">Permissions</span></span>
<span data-ttu-id="ebaf7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebaf7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebaf7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebaf7-110">Permission type</span></span>      | <span data-ttu-id="ebaf7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ebaf7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebaf7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebaf7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ebaf7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebaf7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ebaf7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebaf7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebaf7-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebaf7-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ebaf7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebaf7-116">Application</span></span> | <span data-ttu-id="ebaf7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebaf7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebaf7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="ebaf7-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="ebaf7-119">Optional request headers</span></span>
| <span data-ttu-id="ebaf7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ebaf7-120">Name</span></span>       | <span data-ttu-id="ebaf7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebaf7-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ebaf7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebaf7-122">Authorization</span></span>  | <span data-ttu-id="ebaf7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ebaf7-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ebaf7-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ebaf7-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebaf7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebaf7-128">Request body</span></span>
<span data-ttu-id="ebaf7-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ebaf7-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebaf7-132">Property</span></span>     | <span data-ttu-id="ebaf7-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebaf7-133">Type</span></span>   |<span data-ttu-id="ebaf7-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebaf7-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebaf7-135">position</span><span class="sxs-lookup"><span data-stu-id="ebaf7-135">position</span></span>|<span data-ttu-id="ebaf7-136">string</span><span class="sxs-lookup"><span data-stu-id="ebaf7-136">string</span></span>|<span data-ttu-id="ebaf7-p106">Valor de DataLabelPosition que representa a posição do rótulo de dados. Os valores possíveis são: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit` e `Callout`.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-p106">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="ebaf7-139">separador</span><span class="sxs-lookup"><span data-stu-id="ebaf7-139">separator</span></span>|<span data-ttu-id="ebaf7-140">string</span><span class="sxs-lookup"><span data-stu-id="ebaf7-140">string</span></span>|<span data-ttu-id="ebaf7-141">Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-141">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="ebaf7-142">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="ebaf7-142">showBubbleSize</span></span>|<span data-ttu-id="ebaf7-143">booliano</span><span class="sxs-lookup"><span data-stu-id="ebaf7-143">boolean</span></span>|<span data-ttu-id="ebaf7-144">Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-144">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="ebaf7-145">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="ebaf7-145">showCategoryName</span></span>|<span data-ttu-id="ebaf7-146">booliano</span><span class="sxs-lookup"><span data-stu-id="ebaf7-146">boolean</span></span>|<span data-ttu-id="ebaf7-147">Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-147">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="ebaf7-148">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="ebaf7-148">showLegendKey</span></span>|<span data-ttu-id="ebaf7-149">booliano</span><span class="sxs-lookup"><span data-stu-id="ebaf7-149">boolean</span></span>|<span data-ttu-id="ebaf7-150">Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-150">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="ebaf7-151">showPercentage</span><span class="sxs-lookup"><span data-stu-id="ebaf7-151">showPercentage</span></span>|<span data-ttu-id="ebaf7-152">booliano</span><span class="sxs-lookup"><span data-stu-id="ebaf7-152">boolean</span></span>|<span data-ttu-id="ebaf7-153">Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-153">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="ebaf7-154">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="ebaf7-154">showSeriesName</span></span>|<span data-ttu-id="ebaf7-155">booliano</span><span class="sxs-lookup"><span data-stu-id="ebaf7-155">boolean</span></span>|<span data-ttu-id="ebaf7-156">Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-156">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="ebaf7-157">showValue</span><span class="sxs-lookup"><span data-stu-id="ebaf7-157">showValue</span></span>|<span data-ttu-id="ebaf7-158">booliano</span><span class="sxs-lookup"><span data-stu-id="ebaf7-158">boolean</span></span>|<span data-ttu-id="ebaf7-159">Valor booliano que determina se o valor do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-159">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="ebaf7-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebaf7-160">Response</span></span>

<span data-ttu-id="ebaf7-161">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartDataLabels](../resources/chartdatalabels.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-161">If successful, this method returns a `200 OK` response code and updated [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ebaf7-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebaf7-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebaf7-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebaf7-163">Request</span></span>
<span data-ttu-id="ebaf7-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-164">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ebaf7-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebaf7-165">Response</span></span>
<span data-ttu-id="ebaf7-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebaf7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
