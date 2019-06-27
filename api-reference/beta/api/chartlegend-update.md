---
title: Atualizar chartlegend
description: Atualiza as propriedades do objeto chartlegend.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a942df3d3ee9db7355ffaa9302813571552166b0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261681"
---
# <a name="update-chartlegend"></a><span data-ttu-id="182dd-103">Atualizar chartlegend</span><span class="sxs-lookup"><span data-stu-id="182dd-103">Update chartlegend</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="182dd-104">Atualiza as propriedades do objeto chartlegend.</span><span class="sxs-lookup"><span data-stu-id="182dd-104">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="182dd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="182dd-105">Permissions</span></span>
<span data-ttu-id="182dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="182dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="182dd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="182dd-108">Permission type</span></span>      | <span data-ttu-id="182dd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="182dd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="182dd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="182dd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="182dd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="182dd-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="182dd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="182dd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="182dd-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="182dd-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="182dd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="182dd-114">Application</span></span> | <span data-ttu-id="182dd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="182dd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="182dd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="182dd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="182dd-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="182dd-117">Optional request headers</span></span>
| <span data-ttu-id="182dd-118">Nome</span><span class="sxs-lookup"><span data-stu-id="182dd-118">Name</span></span>       | <span data-ttu-id="182dd-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="182dd-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="182dd-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="182dd-120">Authorization</span></span>  | <span data-ttu-id="182dd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="182dd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="182dd-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="182dd-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="182dd-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="182dd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="182dd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="182dd-126">Request body</span></span>
<span data-ttu-id="182dd-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="182dd-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="182dd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="182dd-130">Property</span></span>     | <span data-ttu-id="182dd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="182dd-131">Type</span></span>   |<span data-ttu-id="182dd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="182dd-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="182dd-133">overlay</span><span class="sxs-lookup"><span data-stu-id="182dd-133">overlay</span></span>|<span data-ttu-id="182dd-134">booliano</span><span class="sxs-lookup"><span data-stu-id="182dd-134">boolean</span></span>|<span data-ttu-id="182dd-135">Valor booliano para determinar se a legenda do gráfico deve se sobrepor ao corpo principal do gráfico.</span><span class="sxs-lookup"><span data-stu-id="182dd-135">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="182dd-136">position</span><span class="sxs-lookup"><span data-stu-id="182dd-136">position</span></span>|<span data-ttu-id="182dd-137">string</span><span class="sxs-lookup"><span data-stu-id="182dd-137">string</span></span>|<span data-ttu-id="182dd-p105">Representa a posição da legenda no gráfico. Os valores possíveis são: `Top`, `Bottom`, `Left`, `Right`, `Corner` e `Custom`.</span><span class="sxs-lookup"><span data-stu-id="182dd-p105">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="182dd-140">visible</span><span class="sxs-lookup"><span data-stu-id="182dd-140">visible</span></span>|<span data-ttu-id="182dd-141">booliano</span><span class="sxs-lookup"><span data-stu-id="182dd-141">boolean</span></span>|<span data-ttu-id="182dd-142">Um valor booliano que representa a visibilidade de um objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="182dd-142">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="182dd-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="182dd-143">Response</span></span>

<span data-ttu-id="182dd-144">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookChartLegend](../resources/workbookchartlegend.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="182dd-144">If successful, this method returns a `200 OK` response code and updated [workbookChartLegend](../resources/workbookchartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="182dd-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="182dd-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="182dd-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="182dd-146">Request</span></span>
<span data-ttu-id="182dd-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="182dd-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="182dd-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="182dd-148">Response</span></span>
<span data-ttu-id="182dd-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="182dd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="182dd-152">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="182dd-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="182dd-153">C#</span><span class="sxs-lookup"><span data-stu-id="182dd-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_chartlegend-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="182dd-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="182dd-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_chartlegend-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="182dd-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="182dd-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_chartlegend-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartlegend-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chartlegend-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chartlegend-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
