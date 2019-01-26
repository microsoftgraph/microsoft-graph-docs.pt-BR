---
title: Tipo de recurso ChartAxis
description: Representa um único eixo em um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d7485c57e45066731eb2e9101840681480ade401
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572819"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="7d3c2-103">Tipo de recurso ChartAxis</span><span class="sxs-lookup"><span data-stu-id="7d3c2-103">ChartAxis resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d3c2-104">Representa um único eixo em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="7d3c2-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="7d3c2-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="7d3c2-105">Methods</span></span>

| <span data-ttu-id="7d3c2-106">Método</span><span class="sxs-lookup"><span data-stu-id="7d3c2-106">Method</span></span>           | <span data-ttu-id="7d3c2-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7d3c2-107">Return Type</span></span>    |<span data-ttu-id="7d3c2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d3c2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7d3c2-109">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="7d3c2-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="7d3c2-110">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="7d3c2-110">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="7d3c2-111">Leia as propriedades e os relacionamentos do objeto chartAxis.</span><span class="sxs-lookup"><span data-stu-id="7d3c2-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="7d3c2-112">Update</span><span class="sxs-lookup"><span data-stu-id="7d3c2-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="7d3c2-113">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="7d3c2-113">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="7d3c2-114">Atualize o objeto ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="7d3c2-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7d3c2-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d3c2-115">Properties</span></span>
| <span data-ttu-id="7d3c2-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d3c2-116">Property</span></span>     | <span data-ttu-id="7d3c2-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d3c2-117">Type</span></span>   |<span data-ttu-id="7d3c2-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d3c2-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7d3c2-119">id</span><span class="sxs-lookup"><span data-stu-id="7d3c2-119">id</span></span>       |<span data-ttu-id="7d3c2-120">string</span><span class="sxs-lookup"><span data-stu-id="7d3c2-120">string</span></span>   | <span data-ttu-id="7d3c2-121">Identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="7d3c2-121">Unique identifier.</span></span> <span data-ttu-id="7d3c2-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d3c2-122">Read-only.</span></span>|
|<span data-ttu-id="7d3c2-123">majorUnit</span><span class="sxs-lookup"><span data-stu-id="7d3c2-123">majorUnit</span></span>|<span data-ttu-id="7d3c2-124">Json</span><span class="sxs-lookup"><span data-stu-id="7d3c2-124">Json</span></span>|<span data-ttu-id="7d3c2-p102">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="7d3c2-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="7d3c2-128">maximum</span><span class="sxs-lookup"><span data-stu-id="7d3c2-128">maximum</span></span>|<span data-ttu-id="7d3c2-129">Json</span><span class="sxs-lookup"><span data-stu-id="7d3c2-129">Json</span></span>|<span data-ttu-id="7d3c2-p103">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="7d3c2-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="7d3c2-133">minimum</span><span class="sxs-lookup"><span data-stu-id="7d3c2-133">minimum</span></span>|<span data-ttu-id="7d3c2-134">Json</span><span class="sxs-lookup"><span data-stu-id="7d3c2-134">Json</span></span>|<span data-ttu-id="7d3c2-p104">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="7d3c2-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="7d3c2-138">minorUnit</span><span class="sxs-lookup"><span data-stu-id="7d3c2-138">minorUnit</span></span>|<span data-ttu-id="7d3c2-139">Json</span><span class="sxs-lookup"><span data-stu-id="7d3c2-139">Json</span></span>|<span data-ttu-id="7d3c2-p105">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="7d3c2-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d3c2-143">Relações</span><span class="sxs-lookup"><span data-stu-id="7d3c2-143">Relationships</span></span>
| <span data-ttu-id="7d3c2-144">Relação</span><span class="sxs-lookup"><span data-stu-id="7d3c2-144">Relationship</span></span> | <span data-ttu-id="7d3c2-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d3c2-145">Type</span></span>   |<span data-ttu-id="7d3c2-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d3c2-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d3c2-147">formato</span><span class="sxs-lookup"><span data-stu-id="7d3c2-147">format</span></span>|[<span data-ttu-id="7d3c2-148">WorkbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="7d3c2-148">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="7d3c2-p106">Representa a formatação de um objeto Chart, que inclui formatação de linha e de fonte. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d3c2-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="7d3c2-151">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="7d3c2-151">majorGridlines</span></span>|[<span data-ttu-id="7d3c2-152">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="7d3c2-152">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="7d3c2-p107">Retorna um objeto de linha de grade que representa as principais linhas de grade do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d3c2-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="7d3c2-155">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="7d3c2-155">minorGridlines</span></span>|[<span data-ttu-id="7d3c2-156">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="7d3c2-156">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="7d3c2-p108">Retorna um objeto Gridlines que representa as linhas de grade secundárias do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d3c2-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="7d3c2-159">title</span><span class="sxs-lookup"><span data-stu-id="7d3c2-159">title</span></span>|[<span data-ttu-id="7d3c2-160">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="7d3c2-160">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="7d3c2-p109">Representa o título do eixo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d3c2-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d3c2-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d3c2-163">JSON representation</span></span>

<span data-ttu-id="7d3c2-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d3c2-164">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxis"
}-->

```json
{
  "id": "string",
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string",
   "format": {"@odata.type": "microsoft.graph.workbookChartAxisFormat"},
  "majorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "minorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "title": {"@odata.type": "microsoft.graph.workbookChartAxisTitle"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxis.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
