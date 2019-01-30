---
title: Atualizar gráfico
description: Atualiza as propriedades do objeto de gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2d1377a0a8c19538ea1c0c19483512736e129559
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640263"
---
# <a name="update-chart"></a><span data-ttu-id="c0b83-103">Atualizar gráfico</span><span class="sxs-lookup"><span data-stu-id="c0b83-103">Update chart</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0b83-104">Atualiza as propriedades do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="c0b83-104">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c0b83-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0b83-105">Permissions</span></span>
<span data-ttu-id="c0b83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0b83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0b83-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0b83-108">Permission type</span></span>      | <span data-ttu-id="c0b83-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0b83-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0b83-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0b83-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c0b83-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0b83-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0b83-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0b83-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0b83-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0b83-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0b83-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0b83-114">Application</span></span> | <span data-ttu-id="c0b83-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0b83-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0b83-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0b83-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="c0b83-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c0b83-117">Optional request headers</span></span>
| <span data-ttu-id="c0b83-118">Name</span><span class="sxs-lookup"><span data-stu-id="c0b83-118">Name</span></span>       | <span data-ttu-id="c0b83-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0b83-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c0b83-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0b83-120">Authorization</span></span>  | <span data-ttu-id="c0b83-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0b83-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c0b83-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c0b83-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c0b83-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c0b83-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0b83-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0b83-126">Request body</span></span>
<span data-ttu-id="c0b83-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c0b83-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c0b83-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0b83-130">Property</span></span>     | <span data-ttu-id="c0b83-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0b83-131">Type</span></span>   |<span data-ttu-id="c0b83-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0b83-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0b83-133">height</span><span class="sxs-lookup"><span data-stu-id="c0b83-133">height</span></span>|<span data-ttu-id="c0b83-134">Double</span><span class="sxs-lookup"><span data-stu-id="c0b83-134">double</span></span>|<span data-ttu-id="c0b83-135">Representa a altura, em pontos, do objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="c0b83-135">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="c0b83-136">left</span><span class="sxs-lookup"><span data-stu-id="c0b83-136">left</span></span>|<span data-ttu-id="c0b83-137">Double</span><span class="sxs-lookup"><span data-stu-id="c0b83-137">double</span></span>|<span data-ttu-id="c0b83-138">A distância, em pontos, da esquerda do gráfico à origem da planilha.</span><span class="sxs-lookup"><span data-stu-id="c0b83-138">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="c0b83-139">name</span><span class="sxs-lookup"><span data-stu-id="c0b83-139">name</span></span>|<span data-ttu-id="c0b83-140">string</span><span class="sxs-lookup"><span data-stu-id="c0b83-140">string</span></span>|<span data-ttu-id="c0b83-141">Representa o nome de um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="c0b83-141">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="c0b83-142">top</span><span class="sxs-lookup"><span data-stu-id="c0b83-142">top</span></span>|<span data-ttu-id="c0b83-143">Double</span><span class="sxs-lookup"><span data-stu-id="c0b83-143">double</span></span>|<span data-ttu-id="c0b83-144">Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="c0b83-144">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="c0b83-145">width</span><span class="sxs-lookup"><span data-stu-id="c0b83-145">width</span></span>|<span data-ttu-id="c0b83-146">Double</span><span class="sxs-lookup"><span data-stu-id="c0b83-146">double</span></span>|<span data-ttu-id="c0b83-147">Representa a largura, em pontos, do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="c0b83-147">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="c0b83-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0b83-148">Response</span></span>

<span data-ttu-id="c0b83-149">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Chart](../resources/chart.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0b83-149">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0b83-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0b83-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0b83-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0b83-151">Request</span></span>
<span data-ttu-id="c0b83-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0b83-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
##### <a name="response"></a><span data-ttu-id="c0b83-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0b83-153">Response</span></span>
<span data-ttu-id="c0b83-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0b83-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
