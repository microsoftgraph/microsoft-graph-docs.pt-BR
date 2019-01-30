---
title: Tipo de recurso ChartAxis
description: Representa um único eixo em um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6cb780272887b6a9b637bbec24b68b37db93657e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640928"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="b202b-103">Tipo de recurso ChartAxis</span><span class="sxs-lookup"><span data-stu-id="b202b-103">ChartAxis resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b202b-104">Representa um único eixo em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="b202b-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="b202b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="b202b-105">Methods</span></span>

| <span data-ttu-id="b202b-106">Método</span><span class="sxs-lookup"><span data-stu-id="b202b-106">Method</span></span>           | <span data-ttu-id="b202b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b202b-107">Return Type</span></span>    |<span data-ttu-id="b202b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b202b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b202b-109">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="b202b-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="b202b-110">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="b202b-110">ChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="b202b-111">Leia as propriedades e os relacionamentos do objeto chartAxis.</span><span class="sxs-lookup"><span data-stu-id="b202b-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="b202b-112">Update</span><span class="sxs-lookup"><span data-stu-id="b202b-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="b202b-113">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="b202b-113">ChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="b202b-114">Atualize o objeto ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="b202b-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b202b-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b202b-115">Properties</span></span>
| <span data-ttu-id="b202b-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b202b-116">Property</span></span>     | <span data-ttu-id="b202b-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="b202b-117">Type</span></span>   |<span data-ttu-id="b202b-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="b202b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b202b-119">majorUnit</span><span class="sxs-lookup"><span data-stu-id="b202b-119">majorUnit</span></span>|<span data-ttu-id="b202b-120">object</span><span class="sxs-lookup"><span data-stu-id="b202b-120">object</span></span>|<span data-ttu-id="b202b-p101">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="b202b-p101">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="b202b-124">maximum</span><span class="sxs-lookup"><span data-stu-id="b202b-124">maximum</span></span>|<span data-ttu-id="b202b-125">object</span><span class="sxs-lookup"><span data-stu-id="b202b-125">object</span></span>|<span data-ttu-id="b202b-p102">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="b202b-p102">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="b202b-129">minimum</span><span class="sxs-lookup"><span data-stu-id="b202b-129">minimum</span></span>|<span data-ttu-id="b202b-130">object</span><span class="sxs-lookup"><span data-stu-id="b202b-130">object</span></span>|<span data-ttu-id="b202b-p103">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="b202b-p103">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="b202b-134">minorUnit</span><span class="sxs-lookup"><span data-stu-id="b202b-134">minorUnit</span></span>|<span data-ttu-id="b202b-135">object</span><span class="sxs-lookup"><span data-stu-id="b202b-135">object</span></span>|<span data-ttu-id="b202b-p104">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="b202b-p104">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b202b-139">Relações</span><span class="sxs-lookup"><span data-stu-id="b202b-139">Relationships</span></span>
| <span data-ttu-id="b202b-140">Relação</span><span class="sxs-lookup"><span data-stu-id="b202b-140">Relationship</span></span> | <span data-ttu-id="b202b-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="b202b-141">Type</span></span>   |<span data-ttu-id="b202b-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="b202b-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b202b-143">formato</span><span class="sxs-lookup"><span data-stu-id="b202b-143">format</span></span>|[<span data-ttu-id="b202b-144">ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="b202b-144">ChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="b202b-p105">Representa a formatação de um objeto Chart, que inclui formatação de linha e de fonte. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b202b-p105">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="b202b-147">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="b202b-147">majorGridlines</span></span>|[<span data-ttu-id="b202b-148">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="b202b-148">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="b202b-p106">Retorna um objeto de linha de grade que representa as principais linhas de grade do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b202b-p106">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="b202b-151">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="b202b-151">minorGridlines</span></span>|[<span data-ttu-id="b202b-152">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="b202b-152">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="b202b-p107">Retorna um objeto Gridlines que representa as linhas de grade secundárias do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b202b-p107">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="b202b-155">title</span><span class="sxs-lookup"><span data-stu-id="b202b-155">title</span></span>|[<span data-ttu-id="b202b-156">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="b202b-156">ChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="b202b-p108">Representa o título do eixo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b202b-p108">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b202b-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b202b-159">JSON representation</span></span>

<span data-ttu-id="b202b-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b202b-160">Here is a JSON representation of the resource.</span></span>

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
