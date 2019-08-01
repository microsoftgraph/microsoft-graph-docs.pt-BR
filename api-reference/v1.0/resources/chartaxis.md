---
title: Tipo de recurso ChartAxis
description: Representa um único eixo em um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 77d688d71757cac9f6d58b9d1bc344d37550e3a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033009"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="c3f63-103">Tipo de recurso ChartAxis</span><span class="sxs-lookup"><span data-stu-id="c3f63-103">ChartAxis resource type</span></span>

<span data-ttu-id="c3f63-104">Representa um único eixo em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="c3f63-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="c3f63-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c3f63-105">Methods</span></span>

| <span data-ttu-id="c3f63-106">Método</span><span class="sxs-lookup"><span data-stu-id="c3f63-106">Method</span></span>           | <span data-ttu-id="c3f63-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c3f63-107">Return Type</span></span>    |<span data-ttu-id="c3f63-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3f63-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c3f63-109">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="c3f63-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="c3f63-110">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="c3f63-110">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="c3f63-111">Leia as propriedades e os relacionamentos do objeto chartAxis.</span><span class="sxs-lookup"><span data-stu-id="c3f63-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="c3f63-112">Update</span><span class="sxs-lookup"><span data-stu-id="c3f63-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="c3f63-113">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="c3f63-113">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="c3f63-114">Atualize o objeto ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="c3f63-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c3f63-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3f63-115">Properties</span></span>
| <span data-ttu-id="c3f63-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3f63-116">Property</span></span>     | <span data-ttu-id="c3f63-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3f63-117">Type</span></span>   |<span data-ttu-id="c3f63-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3f63-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c3f63-119">id</span><span class="sxs-lookup"><span data-stu-id="c3f63-119">id</span></span>       |<span data-ttu-id="c3f63-120">string</span><span class="sxs-lookup"><span data-stu-id="c3f63-120">string</span></span>   | <span data-ttu-id="c3f63-121">Identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="c3f63-121">Unique identifier.</span></span> <span data-ttu-id="c3f63-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3f63-122">Read-only.</span></span>|
|<span data-ttu-id="c3f63-123">majorUnit</span><span class="sxs-lookup"><span data-stu-id="c3f63-123">majorUnit</span></span>|<span data-ttu-id="c3f63-124">Json</span><span class="sxs-lookup"><span data-stu-id="c3f63-124">Json</span></span>|<span data-ttu-id="c3f63-p102">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="c3f63-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="c3f63-128">maximum</span><span class="sxs-lookup"><span data-stu-id="c3f63-128">maximum</span></span>|<span data-ttu-id="c3f63-129">Json</span><span class="sxs-lookup"><span data-stu-id="c3f63-129">Json</span></span>|<span data-ttu-id="c3f63-p103">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="c3f63-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="c3f63-133">minimum</span><span class="sxs-lookup"><span data-stu-id="c3f63-133">minimum</span></span>|<span data-ttu-id="c3f63-134">Json</span><span class="sxs-lookup"><span data-stu-id="c3f63-134">Json</span></span>|<span data-ttu-id="c3f63-p104">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="c3f63-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="c3f63-138">minorUnit</span><span class="sxs-lookup"><span data-stu-id="c3f63-138">minorUnit</span></span>|<span data-ttu-id="c3f63-139">Json</span><span class="sxs-lookup"><span data-stu-id="c3f63-139">Json</span></span>|<span data-ttu-id="c3f63-p105">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="c3f63-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3f63-143">Relações</span><span class="sxs-lookup"><span data-stu-id="c3f63-143">Relationships</span></span>
| <span data-ttu-id="c3f63-144">Relação</span><span class="sxs-lookup"><span data-stu-id="c3f63-144">Relationship</span></span> | <span data-ttu-id="c3f63-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3f63-145">Type</span></span>   |<span data-ttu-id="c3f63-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3f63-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3f63-147">formato</span><span class="sxs-lookup"><span data-stu-id="c3f63-147">format</span></span>|[<span data-ttu-id="c3f63-148">WorkbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="c3f63-148">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="c3f63-p106">Representa a formatação de um objeto Chart, que inclui formatação de linha e de fonte. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3f63-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="c3f63-151">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="c3f63-151">majorGridlines</span></span>|[<span data-ttu-id="c3f63-152">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="c3f63-152">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="c3f63-p107">Retorna um objeto de linha de grade que representa as principais linhas de grade do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3f63-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="c3f63-155">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="c3f63-155">minorGridlines</span></span>|[<span data-ttu-id="c3f63-156">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="c3f63-156">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="c3f63-p108">Retorna um objeto Gridlines que representa as linhas de grade secundárias do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3f63-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="c3f63-159">title</span><span class="sxs-lookup"><span data-stu-id="c3f63-159">title</span></span>|[<span data-ttu-id="c3f63-160">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="c3f63-160">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="c3f63-161">Representa o título do eixo.</span><span class="sxs-lookup"><span data-stu-id="c3f63-161">Represents the axis title.</span></span> <span data-ttu-id="c3f63-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3f63-162">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3f63-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3f63-163">JSON representation</span></span>

<span data-ttu-id="c3f63-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3f63-164">Here is a JSON representation of the resource.</span></span>

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
