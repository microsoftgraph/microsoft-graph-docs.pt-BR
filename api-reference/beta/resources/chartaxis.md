---
title: Tipo de recurso ChartAxis
description: Representa um único eixo em um gráfico.
author: lumine2008
ms.openlocfilehash: 766a1a6823cc83efb3ecaf7250f230216fc13cb0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301824"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="9e61b-103">Tipo de recurso ChartAxis</span><span class="sxs-lookup"><span data-stu-id="9e61b-103">ChartAxis resource type</span></span>

> <span data-ttu-id="9e61b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9e61b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e61b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9e61b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9e61b-106">Representa um único eixo em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="9e61b-106">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="9e61b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="9e61b-107">Methods</span></span>

| <span data-ttu-id="9e61b-108">Método</span><span class="sxs-lookup"><span data-stu-id="9e61b-108">Method</span></span>           | <span data-ttu-id="9e61b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9e61b-109">Return Type</span></span>    |<span data-ttu-id="9e61b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e61b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9e61b-111">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="9e61b-111">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="9e61b-112">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="9e61b-112">ChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="9e61b-113">Leia as propriedades e os relacionamentos do objeto chartAxis.</span><span class="sxs-lookup"><span data-stu-id="9e61b-113">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="9e61b-114">Update</span><span class="sxs-lookup"><span data-stu-id="9e61b-114">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="9e61b-115">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="9e61b-115">ChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="9e61b-116">Atualize o objeto ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="9e61b-116">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9e61b-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e61b-117">Properties</span></span>
| <span data-ttu-id="9e61b-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e61b-118">Property</span></span>     | <span data-ttu-id="9e61b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e61b-119">Type</span></span>   |<span data-ttu-id="9e61b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e61b-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e61b-121">majorUnit</span><span class="sxs-lookup"><span data-stu-id="9e61b-121">majorUnit</span></span>|<span data-ttu-id="9e61b-122">object</span><span class="sxs-lookup"><span data-stu-id="9e61b-122">object</span></span>|<span data-ttu-id="9e61b-p102">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="9e61b-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="9e61b-126">maximum</span><span class="sxs-lookup"><span data-stu-id="9e61b-126">maximum</span></span>|<span data-ttu-id="9e61b-127">object</span><span class="sxs-lookup"><span data-stu-id="9e61b-127">object</span></span>|<span data-ttu-id="9e61b-p103">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="9e61b-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="9e61b-131">minimum</span><span class="sxs-lookup"><span data-stu-id="9e61b-131">minimum</span></span>|<span data-ttu-id="9e61b-132">object</span><span class="sxs-lookup"><span data-stu-id="9e61b-132">object</span></span>|<span data-ttu-id="9e61b-p104">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="9e61b-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="9e61b-136">minorUnit</span><span class="sxs-lookup"><span data-stu-id="9e61b-136">minorUnit</span></span>|<span data-ttu-id="9e61b-137">object</span><span class="sxs-lookup"><span data-stu-id="9e61b-137">object</span></span>|<span data-ttu-id="9e61b-p105">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="9e61b-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e61b-141">Relações</span><span class="sxs-lookup"><span data-stu-id="9e61b-141">Relationships</span></span>
| <span data-ttu-id="9e61b-142">Relação</span><span class="sxs-lookup"><span data-stu-id="9e61b-142">Relationship</span></span> | <span data-ttu-id="9e61b-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e61b-143">Type</span></span>   |<span data-ttu-id="9e61b-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e61b-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e61b-145">formato</span><span class="sxs-lookup"><span data-stu-id="9e61b-145">format</span></span>|[<span data-ttu-id="9e61b-146">ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="9e61b-146">ChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="9e61b-p106">Representa a formatação de um objeto Chart, que inclui formatação de linha e de fonte. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e61b-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="9e61b-149">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="9e61b-149">majorGridlines</span></span>|[<span data-ttu-id="9e61b-150">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="9e61b-150">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="9e61b-p107">Retorna um objeto de linha de grade que representa as principais linhas de grade do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e61b-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="9e61b-153">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="9e61b-153">minorGridlines</span></span>|[<span data-ttu-id="9e61b-154">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="9e61b-154">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="9e61b-p108">Retorna um objeto Gridlines que representa as linhas de grade secundárias do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e61b-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="9e61b-157">title</span><span class="sxs-lookup"><span data-stu-id="9e61b-157">title</span></span>|[<span data-ttu-id="9e61b-158">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="9e61b-158">ChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="9e61b-p109">Representa o título do eixo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e61b-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e61b-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e61b-161">JSON representation</span></span>

<span data-ttu-id="9e61b-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e61b-162">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->