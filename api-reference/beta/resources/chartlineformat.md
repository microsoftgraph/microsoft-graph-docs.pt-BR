---
title: Tipo de recurso ChartLineFormat
description: Abrange as opções de formatação dos elementos de linha.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: b2b7e8bd5c0b489ed42baaa3939f7a839c74c3e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871131"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="81b63-103">Tipo de recurso ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="81b63-103">ChartLineFormat resource type</span></span>

> <span data-ttu-id="81b63-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="81b63-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81b63-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="81b63-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="81b63-106">Abrange as opções de formatação dos elementos de linha.</span><span class="sxs-lookup"><span data-stu-id="81b63-106">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="81b63-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="81b63-107">Methods</span></span>

| <span data-ttu-id="81b63-108">Método</span><span class="sxs-lookup"><span data-stu-id="81b63-108">Method</span></span>           | <span data-ttu-id="81b63-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="81b63-109">Return Type</span></span>    |<span data-ttu-id="81b63-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="81b63-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="81b63-111">Get ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="81b63-111">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="81b63-112">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="81b63-112">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="81b63-113">Leia as propriedades e os relacionamentos do objeto chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="81b63-113">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="81b63-114">Update</span><span class="sxs-lookup"><span data-stu-id="81b63-114">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="81b63-115">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="81b63-115">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="81b63-116">Atualize o objeto ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="81b63-116">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="81b63-117">Clear</span><span class="sxs-lookup"><span data-stu-id="81b63-117">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="81b63-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81b63-118">None</span></span>|<span data-ttu-id="81b63-119">Limpe a formatação da linha de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="81b63-119">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="81b63-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81b63-120">Properties</span></span>
| <span data-ttu-id="81b63-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81b63-121">Property</span></span>     | <span data-ttu-id="81b63-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="81b63-122">Type</span></span>   |<span data-ttu-id="81b63-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="81b63-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81b63-124">color</span><span class="sxs-lookup"><span data-stu-id="81b63-124">color</span></span>|<span data-ttu-id="81b63-125">string</span><span class="sxs-lookup"><span data-stu-id="81b63-125">string</span></span>|<span data-ttu-id="81b63-126">Código de cor HTML que representa a cor das linhas no gráfico.</span><span class="sxs-lookup"><span data-stu-id="81b63-126">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81b63-127">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="81b63-127">Relationships</span></span>
<span data-ttu-id="81b63-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81b63-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="81b63-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81b63-129">JSON representation</span></span>

<span data-ttu-id="81b63-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81b63-130">Here is a JSON representation of the resource.</span></span>

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
