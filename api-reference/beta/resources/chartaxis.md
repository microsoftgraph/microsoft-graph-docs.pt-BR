---
title: Tipo de recurso ChartAxis
description: Representa um único eixo em um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6cb780272887b6a9b637bbec24b68b37db93657e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524720"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="a5da4-103">Tipo de recurso ChartAxis</span><span class="sxs-lookup"><span data-stu-id="a5da4-103">ChartAxis resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5da4-104">Representa um único eixo em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="a5da4-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="a5da4-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="a5da4-105">Methods</span></span>

| <span data-ttu-id="a5da4-106">Método</span><span class="sxs-lookup"><span data-stu-id="a5da4-106">Method</span></span>           | <span data-ttu-id="a5da4-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a5da4-107">Return Type</span></span>    |<span data-ttu-id="a5da4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5da4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5da4-109">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="a5da4-109">[Get ChartAxis](../api/chartaxis-get.md)</span></span> | [<span data-ttu-id="a5da4-110">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="a5da4-110">ChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="a5da4-111">Leia as propriedades e os relacionamentos do objeto chartAxis.</span><span class="sxs-lookup"><span data-stu-id="a5da4-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="a5da4-112">Update</span><span class="sxs-lookup"><span data-stu-id="a5da4-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="a5da4-113">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="a5da4-113">ChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="a5da4-114">Atualize o objeto ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="a5da4-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a5da4-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5da4-115">Properties</span></span>
| <span data-ttu-id="a5da4-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5da4-116">Property</span></span>     | <span data-ttu-id="a5da4-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5da4-117">Type</span></span>   |<span data-ttu-id="a5da4-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5da4-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5da4-119">majorUnit</span><span class="sxs-lookup"><span data-stu-id="a5da4-119">majorUnit</span></span>|<span data-ttu-id="a5da4-120">objeto</span><span class="sxs-lookup"><span data-stu-id="a5da4-120">object</span></span>|<span data-ttu-id="a5da4-p101">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="a5da4-p101">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="a5da4-124">maximum</span><span class="sxs-lookup"><span data-stu-id="a5da4-124">maximum</span></span>|<span data-ttu-id="a5da4-125">objeto</span><span class="sxs-lookup"><span data-stu-id="a5da4-125">object</span></span>|<span data-ttu-id="a5da4-p102">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="a5da4-p102">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="a5da4-129">minimum</span><span class="sxs-lookup"><span data-stu-id="a5da4-129">minimum</span></span>|<span data-ttu-id="a5da4-130">objeto</span><span class="sxs-lookup"><span data-stu-id="a5da4-130">object</span></span>|<span data-ttu-id="a5da4-p103">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="a5da4-p103">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="a5da4-134">minorUnit</span><span class="sxs-lookup"><span data-stu-id="a5da4-134">minorUnit</span></span>|<span data-ttu-id="a5da4-135">object</span><span class="sxs-lookup"><span data-stu-id="a5da4-135">object</span></span>|<span data-ttu-id="a5da4-p104">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="a5da4-p104">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5da4-139">Relações</span><span class="sxs-lookup"><span data-stu-id="a5da4-139">Relationships</span></span>
| <span data-ttu-id="a5da4-140">Relação</span><span class="sxs-lookup"><span data-stu-id="a5da4-140">Relationship</span></span> | <span data-ttu-id="a5da4-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5da4-141">Type</span></span>   |<span data-ttu-id="a5da4-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5da4-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5da4-143">formato</span><span class="sxs-lookup"><span data-stu-id="a5da4-143">format</span></span>|[<span data-ttu-id="a5da4-144">ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="a5da4-144">ChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="a5da4-p105">Representa a formatação de um objeto Chart, que inclui formatação de linha e de fonte. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a5da4-p105">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="a5da4-147">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="a5da4-147">majorGridlines</span></span>|<span data-ttu-id="a5da4-148">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="a5da4-148">[ChartGridlines](chartgridlines.md)</span></span>|<span data-ttu-id="a5da4-p106">Retorna um objeto de linha de grade que representa as principais linhas de grade do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a5da4-p106">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="a5da4-151">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="a5da4-151">minorGridlines</span></span>|[<span data-ttu-id="a5da4-152">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="a5da4-152">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="a5da4-p107">Retorna um objeto Gridlines que representa as linhas de grade secundárias do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a5da4-p107">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="a5da4-155">title</span><span class="sxs-lookup"><span data-stu-id="a5da4-155">title</span></span>|[<span data-ttu-id="a5da4-156">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="a5da4-156">ChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="a5da4-p108">Representa o título do eixo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a5da4-p108">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5da4-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5da4-159">JSON representation</span></span>

<span data-ttu-id="a5da4-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a5da4-160">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartaxis"
}-->

```json
{
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string"
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
