---
title: tipo de recurso workbookChartAxis
description: Representa um único eixo em um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ce18f029e3e5e48597ac5074d683e6a8cdb64674
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348465"
---
# <a name="workbookchartaxis-resource-type"></a><span data-ttu-id="087a1-103">tipo de recurso workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="087a1-103">workbookChartAxis resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="087a1-104">Representa um único eixo em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="087a1-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="087a1-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="087a1-105">Methods</span></span>

| <span data-ttu-id="087a1-106">Método</span><span class="sxs-lookup"><span data-stu-id="087a1-106">Method</span></span>           | <span data-ttu-id="087a1-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="087a1-107">Return Type</span></span>    |<span data-ttu-id="087a1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="087a1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="087a1-109">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="087a1-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="087a1-110">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="087a1-110">workbookChartAxis</span></span>](workbookchartaxis.md) |<span data-ttu-id="087a1-111">Leia as propriedades e os relacionamentos do objeto chartAxis.</span><span class="sxs-lookup"><span data-stu-id="087a1-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="087a1-112">Update</span><span class="sxs-lookup"><span data-stu-id="087a1-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="087a1-113">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="087a1-113">workbookChartAxis</span></span>](workbookchartaxis.md)   |<span data-ttu-id="087a1-114">Atualize o objeto ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="087a1-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="087a1-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="087a1-115">Properties</span></span>
| <span data-ttu-id="087a1-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="087a1-116">Property</span></span>     | <span data-ttu-id="087a1-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="087a1-117">Type</span></span>   |<span data-ttu-id="087a1-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="087a1-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="087a1-119">id</span><span class="sxs-lookup"><span data-stu-id="087a1-119">id</span></span>       |<span data-ttu-id="087a1-120">string</span><span class="sxs-lookup"><span data-stu-id="087a1-120">string</span></span>   | <span data-ttu-id="087a1-121">Identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="087a1-121">Unique identifier.</span></span> <span data-ttu-id="087a1-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="087a1-122">Read-only.</span></span>|
|<span data-ttu-id="087a1-123">majorUnit</span><span class="sxs-lookup"><span data-stu-id="087a1-123">majorUnit</span></span>|<span data-ttu-id="087a1-124">Json</span><span class="sxs-lookup"><span data-stu-id="087a1-124">Json</span></span>|<span data-ttu-id="087a1-p102">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="087a1-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="087a1-128">maximum</span><span class="sxs-lookup"><span data-stu-id="087a1-128">maximum</span></span>|<span data-ttu-id="087a1-129">Json</span><span class="sxs-lookup"><span data-stu-id="087a1-129">Json</span></span>|<span data-ttu-id="087a1-p103">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="087a1-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="087a1-133">minimum</span><span class="sxs-lookup"><span data-stu-id="087a1-133">minimum</span></span>|<span data-ttu-id="087a1-134">Json</span><span class="sxs-lookup"><span data-stu-id="087a1-134">Json</span></span>|<span data-ttu-id="087a1-p104">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="087a1-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="087a1-138">minorUnit</span><span class="sxs-lookup"><span data-stu-id="087a1-138">minorUnit</span></span>|<span data-ttu-id="087a1-139">Json</span><span class="sxs-lookup"><span data-stu-id="087a1-139">Json</span></span>|<span data-ttu-id="087a1-p105">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="087a1-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="087a1-143">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="087a1-143">Relationships</span></span>
| <span data-ttu-id="087a1-144">Relação</span><span class="sxs-lookup"><span data-stu-id="087a1-144">Relationship</span></span> | <span data-ttu-id="087a1-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="087a1-145">Type</span></span>   |<span data-ttu-id="087a1-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="087a1-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="087a1-147">formato</span><span class="sxs-lookup"><span data-stu-id="087a1-147">format</span></span>|[<span data-ttu-id="087a1-148">workbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="087a1-148">workbookChartAxisFormat</span></span>](workbookchartaxisformat.md)|<span data-ttu-id="087a1-p106">Representa a formatação de um objeto Chart, que inclui formatação de linha e de fonte. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="087a1-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="087a1-151">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="087a1-151">majorGridlines</span></span>|[<span data-ttu-id="087a1-152">workbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="087a1-152">workbookChartGridlines</span></span>](workbookchartgridlines.md)|<span data-ttu-id="087a1-p107">Retorna um objeto de linha de grade que representa as principais linhas de grade do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="087a1-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="087a1-155">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="087a1-155">minorGridlines</span></span>|[<span data-ttu-id="087a1-156">workbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="087a1-156">workbookChartGridlines</span></span>](workbookchartgridlines.md)|<span data-ttu-id="087a1-p108">Retorna um objeto Gridlines que representa as linhas de grade secundárias do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="087a1-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="087a1-159">title</span><span class="sxs-lookup"><span data-stu-id="087a1-159">title</span></span>|[<span data-ttu-id="087a1-160">workbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="087a1-160">workbookChartAxisTitle</span></span>](workbookchartaxistitle.md)|<span data-ttu-id="087a1-161">Representa o título do eixo.</span><span class="sxs-lookup"><span data-stu-id="087a1-161">Represents the axis title.</span></span> <span data-ttu-id="087a1-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="087a1-162">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="087a1-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="087a1-163">JSON representation</span></span>

<span data-ttu-id="087a1-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="087a1-164">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "title",
    "minorGridlines",
    "majorGridlines",
    "format"
   ],
  "keyProperty": "id",
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
  "suppressions": []
}
-->
