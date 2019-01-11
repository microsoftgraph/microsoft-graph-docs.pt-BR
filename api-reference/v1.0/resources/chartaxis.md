---
title: Tipo de recurso ChartAxis
description: Representa um único eixo em um gráfico.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 57c8e28633d4fc60f60f456e34a6a0cafef22252
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829082"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="aca3b-103">Tipo de recurso ChartAxis</span><span class="sxs-lookup"><span data-stu-id="aca3b-103">ChartAxis resource type</span></span>

<span data-ttu-id="aca3b-104">Representa um único eixo em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="aca3b-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="aca3b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="aca3b-105">Methods</span></span>

| <span data-ttu-id="aca3b-106">Método</span><span class="sxs-lookup"><span data-stu-id="aca3b-106">Method</span></span>           | <span data-ttu-id="aca3b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="aca3b-107">Return Type</span></span>    |<span data-ttu-id="aca3b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="aca3b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aca3b-109">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="aca3b-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="aca3b-110">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="aca3b-110">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="aca3b-111">Leia as propriedades e os relacionamentos do objeto chartAxis.</span><span class="sxs-lookup"><span data-stu-id="aca3b-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="aca3b-112">Update</span><span class="sxs-lookup"><span data-stu-id="aca3b-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="aca3b-113">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="aca3b-113">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="aca3b-114">Atualize o objeto ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="aca3b-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="aca3b-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aca3b-115">Properties</span></span>
| <span data-ttu-id="aca3b-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aca3b-116">Property</span></span>     | <span data-ttu-id="aca3b-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="aca3b-117">Type</span></span>   |<span data-ttu-id="aca3b-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="aca3b-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aca3b-119">id</span><span class="sxs-lookup"><span data-stu-id="aca3b-119">id</span></span>       |<span data-ttu-id="aca3b-120">string</span><span class="sxs-lookup"><span data-stu-id="aca3b-120">string</span></span>   | <span data-ttu-id="aca3b-121">Identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="aca3b-121">Unique identifier.</span></span> <span data-ttu-id="aca3b-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aca3b-122">Read-only.</span></span>|
|<span data-ttu-id="aca3b-123">majorUnit</span><span class="sxs-lookup"><span data-stu-id="aca3b-123">majorUnit</span></span>|<span data-ttu-id="aca3b-124">Json</span><span class="sxs-lookup"><span data-stu-id="aca3b-124">Json</span></span>|<span data-ttu-id="aca3b-p102">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="aca3b-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="aca3b-128">maximum</span><span class="sxs-lookup"><span data-stu-id="aca3b-128">maximum</span></span>|<span data-ttu-id="aca3b-129">Json</span><span class="sxs-lookup"><span data-stu-id="aca3b-129">Json</span></span>|<span data-ttu-id="aca3b-p103">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="aca3b-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="aca3b-133">minimum</span><span class="sxs-lookup"><span data-stu-id="aca3b-133">minimum</span></span>|<span data-ttu-id="aca3b-134">Json</span><span class="sxs-lookup"><span data-stu-id="aca3b-134">Json</span></span>|<span data-ttu-id="aca3b-p104">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="aca3b-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="aca3b-138">minorUnit</span><span class="sxs-lookup"><span data-stu-id="aca3b-138">minorUnit</span></span>|<span data-ttu-id="aca3b-139">Json</span><span class="sxs-lookup"><span data-stu-id="aca3b-139">Json</span></span>|<span data-ttu-id="aca3b-p105">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="aca3b-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aca3b-143">Relações</span><span class="sxs-lookup"><span data-stu-id="aca3b-143">Relationships</span></span>
| <span data-ttu-id="aca3b-144">Relação</span><span class="sxs-lookup"><span data-stu-id="aca3b-144">Relationship</span></span> | <span data-ttu-id="aca3b-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="aca3b-145">Type</span></span>   |<span data-ttu-id="aca3b-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="aca3b-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aca3b-147">formato</span><span class="sxs-lookup"><span data-stu-id="aca3b-147">format</span></span>|[<span data-ttu-id="aca3b-148">WorkbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="aca3b-148">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="aca3b-p106">Representa a formatação de um objeto Chart, que inclui formatação de linha e de fonte. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aca3b-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="aca3b-151">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="aca3b-151">majorGridlines</span></span>|[<span data-ttu-id="aca3b-152">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="aca3b-152">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="aca3b-p107">Retorna um objeto de linha de grade que representa as principais linhas de grade do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aca3b-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="aca3b-155">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="aca3b-155">minorGridlines</span></span>|[<span data-ttu-id="aca3b-156">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="aca3b-156">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="aca3b-p108">Retorna um objeto Gridlines que representa as linhas de grade secundárias do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aca3b-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="aca3b-159">título</span><span class="sxs-lookup"><span data-stu-id="aca3b-159">title</span></span>|[<span data-ttu-id="aca3b-160">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="aca3b-160">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="aca3b-p109">Representa o título do eixo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aca3b-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aca3b-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aca3b-163">JSON representation</span></span>

<span data-ttu-id="aca3b-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aca3b-164">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
