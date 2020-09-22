---
title: tipo de recurso workbookChartAxis
description: Representa um único eixo em um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ca26aec49744bacf1e9e1d9738dfd552944622f7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039079"
---
# <a name="workbookchartaxis-resource-type"></a><span data-ttu-id="f4fad-103">tipo de recurso workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="f4fad-103">workbookChartAxis resource type</span></span>

<span data-ttu-id="f4fad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4fad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4fad-105">Representa um único eixo em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="f4fad-105">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="f4fad-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f4fad-106">Methods</span></span>

| <span data-ttu-id="f4fad-107">Método</span><span class="sxs-lookup"><span data-stu-id="f4fad-107">Method</span></span>           | <span data-ttu-id="f4fad-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f4fad-108">Return Type</span></span>    |<span data-ttu-id="f4fad-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4fad-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f4fad-110">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="f4fad-110">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="f4fad-111">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="f4fad-111">workbookChartAxis</span></span>](workbookchartaxis.md) |<span data-ttu-id="f4fad-112">Leia as propriedades e os relacionamentos do objeto chartAxis.</span><span class="sxs-lookup"><span data-stu-id="f4fad-112">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="f4fad-113">Update</span><span class="sxs-lookup"><span data-stu-id="f4fad-113">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="f4fad-114">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="f4fad-114">workbookChartAxis</span></span>](workbookchartaxis.md)   |<span data-ttu-id="f4fad-115">Atualize o objeto ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="f4fad-115">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f4fad-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4fad-116">Properties</span></span>
| <span data-ttu-id="f4fad-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4fad-117">Property</span></span>     | <span data-ttu-id="f4fad-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4fad-118">Type</span></span>   |<span data-ttu-id="f4fad-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4fad-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f4fad-120">id</span><span class="sxs-lookup"><span data-stu-id="f4fad-120">id</span></span>       |<span data-ttu-id="f4fad-121">string</span><span class="sxs-lookup"><span data-stu-id="f4fad-121">string</span></span>   | <span data-ttu-id="f4fad-122">Identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="f4fad-122">Unique identifier.</span></span> <span data-ttu-id="f4fad-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4fad-123">Read-only.</span></span>|
|<span data-ttu-id="f4fad-124">majorUnit</span><span class="sxs-lookup"><span data-stu-id="f4fad-124">majorUnit</span></span>|<span data-ttu-id="f4fad-125">Json</span><span class="sxs-lookup"><span data-stu-id="f4fad-125">Json</span></span>|<span data-ttu-id="f4fad-p102">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="f4fad-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="f4fad-129">maximum</span><span class="sxs-lookup"><span data-stu-id="f4fad-129">maximum</span></span>|<span data-ttu-id="f4fad-130">Json</span><span class="sxs-lookup"><span data-stu-id="f4fad-130">Json</span></span>|<span data-ttu-id="f4fad-p103">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="f4fad-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="f4fad-134">minimum</span><span class="sxs-lookup"><span data-stu-id="f4fad-134">minimum</span></span>|<span data-ttu-id="f4fad-135">Json</span><span class="sxs-lookup"><span data-stu-id="f4fad-135">Json</span></span>|<span data-ttu-id="f4fad-p104">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="f4fad-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="f4fad-139">minorUnit</span><span class="sxs-lookup"><span data-stu-id="f4fad-139">minorUnit</span></span>|<span data-ttu-id="f4fad-140">Json</span><span class="sxs-lookup"><span data-stu-id="f4fad-140">Json</span></span>|<span data-ttu-id="f4fad-p105">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="f4fad-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4fad-144">Relações</span><span class="sxs-lookup"><span data-stu-id="f4fad-144">Relationships</span></span>
| <span data-ttu-id="f4fad-145">Relação</span><span class="sxs-lookup"><span data-stu-id="f4fad-145">Relationship</span></span> | <span data-ttu-id="f4fad-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4fad-146">Type</span></span>   |<span data-ttu-id="f4fad-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4fad-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4fad-148">formato</span><span class="sxs-lookup"><span data-stu-id="f4fad-148">format</span></span>|[<span data-ttu-id="f4fad-149">workbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="f4fad-149">workbookChartAxisFormat</span></span>](workbookchartaxisformat.md)|<span data-ttu-id="f4fad-p106">Representa a formatação de um objeto Chart, que inclui formatação de linha e de fonte. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4fad-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="f4fad-152">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="f4fad-152">majorGridlines</span></span>|[<span data-ttu-id="f4fad-153">workbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="f4fad-153">workbookChartGridlines</span></span>](workbookchartgridlines.md)|<span data-ttu-id="f4fad-p107">Retorna um objeto de linha de grade que representa as principais linhas de grade do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4fad-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="f4fad-156">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="f4fad-156">minorGridlines</span></span>|[<span data-ttu-id="f4fad-157">workbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="f4fad-157">workbookChartGridlines</span></span>](workbookchartgridlines.md)|<span data-ttu-id="f4fad-p108">Retorna um objeto Gridlines que representa as linhas de grade secundárias do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4fad-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="f4fad-160">title</span><span class="sxs-lookup"><span data-stu-id="f4fad-160">title</span></span>|[<span data-ttu-id="f4fad-161">workbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="f4fad-161">workbookChartAxisTitle</span></span>](workbookchartaxistitle.md)|<span data-ttu-id="f4fad-162">Representa o título do eixo.</span><span class="sxs-lookup"><span data-stu-id="f4fad-162">Represents the axis title.</span></span> <span data-ttu-id="f4fad-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4fad-163">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4fad-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4fad-164">JSON representation</span></span>

<span data-ttu-id="f4fad-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4fad-165">Here is a JSON representation of the resource.</span></span>

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


