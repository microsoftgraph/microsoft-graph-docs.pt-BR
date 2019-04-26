---
title: 'workbookChartCollection: Adicionar'
description: Cria um novo workbookChart.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2ee41230d153fb02c3165062ff054a2b3fe4e2a6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327826"
---
# <a name="workbookchartcollection-add"></a><span data-ttu-id="96d3e-103">workbookChartCollection: Adicionar</span><span class="sxs-lookup"><span data-stu-id="96d3e-103">workbookChartCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96d3e-104">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="96d3e-104">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="96d3e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="96d3e-105">Permissions</span></span>
<span data-ttu-id="96d3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96d3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96d3e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96d3e-108">Permission type</span></span>      | <span data-ttu-id="96d3e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96d3e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96d3e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96d3e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96d3e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96d3e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="96d3e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96d3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96d3e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96d3e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="96d3e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96d3e-114">Application</span></span> | <span data-ttu-id="96d3e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96d3e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96d3e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96d3e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="96d3e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96d3e-117">Request headers</span></span>
| <span data-ttu-id="96d3e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="96d3e-118">Name</span></span>       | <span data-ttu-id="96d3e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="96d3e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="96d3e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="96d3e-120">Authorization</span></span>  | <span data-ttu-id="96d3e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96d3e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96d3e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="96d3e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="96d3e-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="96d3e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96d3e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96d3e-126">Request body</span></span>
<span data-ttu-id="96d3e-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96d3e-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="96d3e-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="96d3e-128">Parameter</span></span>    | <span data-ttu-id="96d3e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="96d3e-129">Type</span></span>   |<span data-ttu-id="96d3e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="96d3e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96d3e-131">type</span><span class="sxs-lookup"><span data-stu-id="96d3e-131">type</span></span>|<span data-ttu-id="96d3e-132">string</span><span class="sxs-lookup"><span data-stu-id="96d3e-132">string</span></span>|<span data-ttu-id="96d3e-133">Representa o tipo de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="96d3e-133">Represents the type of a chart.</span></span>  <span data-ttu-id="96d3e-134">Os valores possíveis são: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span><span class="sxs-lookup"><span data-stu-id="96d3e-134">The possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="96d3e-135">sourceData</span><span class="sxs-lookup"><span data-stu-id="96d3e-135">sourceData</span></span>|<span data-ttu-id="96d3e-136">Json</span><span class="sxs-lookup"><span data-stu-id="96d3e-136">Json</span></span>|<span data-ttu-id="96d3e-137">O objeto Range correspondente aos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="96d3e-137">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="96d3e-138">seriesBy</span><span class="sxs-lookup"><span data-stu-id="96d3e-138">seriesBy</span></span>|<span data-ttu-id="96d3e-139">string</span><span class="sxs-lookup"><span data-stu-id="96d3e-139">string</span></span>|<span data-ttu-id="96d3e-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="96d3e-140">Optional.</span></span> <span data-ttu-id="96d3e-141">Especifica a forma como as colunas ou linhas são usadas como série de dados no gráfico.</span><span class="sxs-lookup"><span data-stu-id="96d3e-141">Specifies the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="96d3e-142">Os valores possíveis são: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="96d3e-142">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="96d3e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="96d3e-143">Response</span></span>

<span data-ttu-id="96d3e-144">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [workbookChart](../resources/workbookchart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96d3e-144">If successful, this method returns `200 OK` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96d3e-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96d3e-145">Example</span></span>
<span data-ttu-id="96d3e-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="96d3e-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="96d3e-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96d3e-147">Request</span></span>
<span data-ttu-id="96d3e-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96d3e-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```

##### <a name="response"></a><span data-ttu-id="96d3e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="96d3e-149">Response</span></span>
<span data-ttu-id="96d3e-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96d3e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
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
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
