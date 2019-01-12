---
title: Tipo de recurso ChartAxis
description: Representa um único eixo em um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c6344f2bbb102e2e2402dba267538cb46d4c0fbe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914189"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="819ce-103">Tipo de recurso ChartAxis</span><span class="sxs-lookup"><span data-stu-id="819ce-103">ChartAxis resource type</span></span>

> <span data-ttu-id="819ce-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="819ce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="819ce-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="819ce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="819ce-106">Representa um único eixo em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="819ce-106">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="819ce-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="819ce-107">Methods</span></span>

| <span data-ttu-id="819ce-108">Método</span><span class="sxs-lookup"><span data-stu-id="819ce-108">Method</span></span>           | <span data-ttu-id="819ce-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="819ce-109">Return Type</span></span>    |<span data-ttu-id="819ce-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="819ce-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="819ce-111">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="819ce-111">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="819ce-112">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="819ce-112">ChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="819ce-113">Leia as propriedades e os relacionamentos do objeto chartAxis.</span><span class="sxs-lookup"><span data-stu-id="819ce-113">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="819ce-114">Update</span><span class="sxs-lookup"><span data-stu-id="819ce-114">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="819ce-115">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="819ce-115">ChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="819ce-116">Atualize o objeto ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="819ce-116">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="819ce-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="819ce-117">Properties</span></span>
| <span data-ttu-id="819ce-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="819ce-118">Property</span></span>     | <span data-ttu-id="819ce-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="819ce-119">Type</span></span>   |<span data-ttu-id="819ce-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="819ce-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="819ce-121">majorUnit</span><span class="sxs-lookup"><span data-stu-id="819ce-121">majorUnit</span></span>|<span data-ttu-id="819ce-122">object</span><span class="sxs-lookup"><span data-stu-id="819ce-122">object</span></span>|<span data-ttu-id="819ce-p102">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="819ce-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="819ce-126">maximum</span><span class="sxs-lookup"><span data-stu-id="819ce-126">maximum</span></span>|<span data-ttu-id="819ce-127">object</span><span class="sxs-lookup"><span data-stu-id="819ce-127">object</span></span>|<span data-ttu-id="819ce-p103">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="819ce-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="819ce-131">minimum</span><span class="sxs-lookup"><span data-stu-id="819ce-131">minimum</span></span>|<span data-ttu-id="819ce-132">object</span><span class="sxs-lookup"><span data-stu-id="819ce-132">object</span></span>|<span data-ttu-id="819ce-p104">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="819ce-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="819ce-136">minorUnit</span><span class="sxs-lookup"><span data-stu-id="819ce-136">minorUnit</span></span>|<span data-ttu-id="819ce-137">object</span><span class="sxs-lookup"><span data-stu-id="819ce-137">object</span></span>|<span data-ttu-id="819ce-p105">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="819ce-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="819ce-141">Relações</span><span class="sxs-lookup"><span data-stu-id="819ce-141">Relationships</span></span>
| <span data-ttu-id="819ce-142">Relação</span><span class="sxs-lookup"><span data-stu-id="819ce-142">Relationship</span></span> | <span data-ttu-id="819ce-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="819ce-143">Type</span></span>   |<span data-ttu-id="819ce-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="819ce-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="819ce-145">formato</span><span class="sxs-lookup"><span data-stu-id="819ce-145">format</span></span>|[<span data-ttu-id="819ce-146">ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="819ce-146">ChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="819ce-p106">Representa a formatação de um objeto Chart, que inclui formatação de linha e de fonte. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="819ce-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="819ce-149">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="819ce-149">majorGridlines</span></span>|[<span data-ttu-id="819ce-150">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="819ce-150">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="819ce-p107">Retorna um objeto de linha de grade que representa as principais linhas de grade do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="819ce-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="819ce-153">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="819ce-153">minorGridlines</span></span>|[<span data-ttu-id="819ce-154">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="819ce-154">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="819ce-p108">Retorna um objeto Gridlines que representa as linhas de grade secundárias do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="819ce-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="819ce-157">título</span><span class="sxs-lookup"><span data-stu-id="819ce-157">title</span></span>|[<span data-ttu-id="819ce-158">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="819ce-158">ChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="819ce-p109">Representa o título do eixo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="819ce-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="819ce-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="819ce-161">JSON representation</span></span>

<span data-ttu-id="819ce-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="819ce-162">Here is a JSON representation of the resource.</span></span>

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
