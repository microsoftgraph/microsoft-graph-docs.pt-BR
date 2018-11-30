---
title: Tipo de recurso ChartLineFormat
description: Abrange as opções de formatação dos elementos de linha.
ms.openlocfilehash: 6646f985fd106ed738432852fec5a3bad187ab61
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037147"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="964ee-103">Tipo de recurso ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="964ee-103">ChartLineFormat resource type</span></span>

> <span data-ttu-id="964ee-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="964ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="964ee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="964ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="964ee-106">Abrange as opções de formatação dos elementos de linha.</span><span class="sxs-lookup"><span data-stu-id="964ee-106">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="964ee-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="964ee-107">Methods</span></span>

| <span data-ttu-id="964ee-108">Método</span><span class="sxs-lookup"><span data-stu-id="964ee-108">Method</span></span>           | <span data-ttu-id="964ee-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="964ee-109">Return Type</span></span>    |<span data-ttu-id="964ee-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="964ee-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="964ee-111">Get ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="964ee-111">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="964ee-112">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="964ee-112">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="964ee-113">Leia as propriedades e os relacionamentos do objeto chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="964ee-113">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="964ee-114">Update</span><span class="sxs-lookup"><span data-stu-id="964ee-114">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="964ee-115">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="964ee-115">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="964ee-116">Atualize o objeto ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="964ee-116">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="964ee-117">Clear</span><span class="sxs-lookup"><span data-stu-id="964ee-117">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="964ee-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="964ee-118">None</span></span>|<span data-ttu-id="964ee-119">Limpe a formatação da linha de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="964ee-119">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="964ee-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="964ee-120">Properties</span></span>
| <span data-ttu-id="964ee-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="964ee-121">Property</span></span>     | <span data-ttu-id="964ee-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="964ee-122">Type</span></span>   |<span data-ttu-id="964ee-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="964ee-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="964ee-124">color</span><span class="sxs-lookup"><span data-stu-id="964ee-124">color</span></span>|<span data-ttu-id="964ee-125">string</span><span class="sxs-lookup"><span data-stu-id="964ee-125">string</span></span>|<span data-ttu-id="964ee-126">Código de cor HTML que representa a cor das linhas no gráfico.</span><span class="sxs-lookup"><span data-stu-id="964ee-126">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="964ee-127">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="964ee-127">Relationships</span></span>
<span data-ttu-id="964ee-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="964ee-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="964ee-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="964ee-129">JSON representation</span></span>

<span data-ttu-id="964ee-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="964ee-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->