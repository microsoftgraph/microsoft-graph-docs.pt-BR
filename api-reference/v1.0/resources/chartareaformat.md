---
title: Tipo de recurso ChartAreaFormat
description: Encapsula as propriedades de formato da área de gráfico geral.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 1a864dfb960a17ec4ea3d27dc114284d14f08789
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531913"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="b8dff-103">Tipo de recurso ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="b8dff-103">ChartAreaFormat resource type</span></span>

<span data-ttu-id="b8dff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8dff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8dff-105">Encapsula as propriedades de formato da área de gráfico geral.</span><span class="sxs-lookup"><span data-stu-id="b8dff-105">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="b8dff-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b8dff-106">Methods</span></span>
<span data-ttu-id="b8dff-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8dff-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="b8dff-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8dff-108">Properties</span></span>
<span data-ttu-id="b8dff-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b8dff-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="b8dff-110">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="b8dff-110">Relationships</span></span>
| <span data-ttu-id="b8dff-111">Relação</span><span class="sxs-lookup"><span data-stu-id="b8dff-111">Relationship</span></span> | <span data-ttu-id="b8dff-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8dff-112">Type</span></span>   |<span data-ttu-id="b8dff-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8dff-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8dff-114">fill</span><span class="sxs-lookup"><span data-stu-id="b8dff-114">fill</span></span>|[<span data-ttu-id="b8dff-115">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="b8dff-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="b8dff-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b8dff-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="b8dff-118">font</span><span class="sxs-lookup"><span data-stu-id="b8dff-118">font</span></span>|[<span data-ttu-id="b8dff-119">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="b8dff-119">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="b8dff-120">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="b8dff-120">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="b8dff-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b8dff-121">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8dff-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8dff-122">JSON representation</span></span>

<span data-ttu-id="b8dff-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8dff-123">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAreaFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
