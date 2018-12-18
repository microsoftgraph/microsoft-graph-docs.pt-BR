---
title: Tipo de recurso ChartAxisTitle
description: Representa o título de um eixo do gráfico.
author: lumine2008
ms.openlocfilehash: f787e4572c0b0f499740e2ba1e790fec1ce7ba61
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357292"
---
# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="fe90e-103">Tipo de recurso ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="fe90e-103">ChartAxisTitle resource type</span></span>

> <span data-ttu-id="fe90e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fe90e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe90e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fe90e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe90e-106">Representa o título de um eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="fe90e-106">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="fe90e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="fe90e-107">Methods</span></span>

| <span data-ttu-id="fe90e-108">Método</span><span class="sxs-lookup"><span data-stu-id="fe90e-108">Method</span></span>           | <span data-ttu-id="fe90e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fe90e-109">Return Type</span></span>    |<span data-ttu-id="fe90e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe90e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fe90e-111">Get ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="fe90e-111">Get ChartAxisTitle</span></span>](../api/chartaxistitle-get.md) | [<span data-ttu-id="fe90e-112">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="fe90e-112">ChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="fe90e-113">Recupere as propriedades e os relacionamentos do objeto chartAxisTitle.</span><span class="sxs-lookup"><span data-stu-id="fe90e-113">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="fe90e-114">Update</span><span class="sxs-lookup"><span data-stu-id="fe90e-114">Update</span></span>](../api/chartaxistitle-update.md) | [<span data-ttu-id="fe90e-115">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="fe90e-115">ChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="fe90e-116">Atualize o objeto ChartAxisTitle.</span><span class="sxs-lookup"><span data-stu-id="fe90e-116">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fe90e-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe90e-117">Properties</span></span>
| <span data-ttu-id="fe90e-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe90e-118">Property</span></span>     | <span data-ttu-id="fe90e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe90e-119">Type</span></span>   |<span data-ttu-id="fe90e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe90e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe90e-121">texto</span><span class="sxs-lookup"><span data-stu-id="fe90e-121">text</span></span>|<span data-ttu-id="fe90e-122">string</span><span class="sxs-lookup"><span data-stu-id="fe90e-122">string</span></span>|<span data-ttu-id="fe90e-123">Representa o título do eixo.</span><span class="sxs-lookup"><span data-stu-id="fe90e-123">Represents the axis title.</span></span>|
|<span data-ttu-id="fe90e-124">visible</span><span class="sxs-lookup"><span data-stu-id="fe90e-124">visible</span></span>|<span data-ttu-id="fe90e-125">booliano</span><span class="sxs-lookup"><span data-stu-id="fe90e-125">boolean</span></span>|<span data-ttu-id="fe90e-126">Um booliano que especifica a visibilidade de um título do eixo.</span><span class="sxs-lookup"><span data-stu-id="fe90e-126">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe90e-127">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="fe90e-127">Relationships</span></span>
| <span data-ttu-id="fe90e-128">Relação</span><span class="sxs-lookup"><span data-stu-id="fe90e-128">Relationship</span></span> | <span data-ttu-id="fe90e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe90e-129">Type</span></span>   |<span data-ttu-id="fe90e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe90e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe90e-131">formato</span><span class="sxs-lookup"><span data-stu-id="fe90e-131">format</span></span>|[<span data-ttu-id="fe90e-132">ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="fe90e-132">ChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="fe90e-p102">Representa a formatação do título do eixo do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fe90e-p102">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe90e-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe90e-135">JSON representation</span></span>

<span data-ttu-id="fe90e-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe90e-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->