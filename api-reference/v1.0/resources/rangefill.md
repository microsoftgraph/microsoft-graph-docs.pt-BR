---
title: Tipo de recurso RangeFill
description: Representa o plano de fundo de um objeto de intervalo.
ms.openlocfilehash: 7a9919d5190c34937319de1c15f722453b7c79e0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003998"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="e9aba-103">Tipo de recurso RangeFill</span><span class="sxs-lookup"><span data-stu-id="e9aba-103">RangeFill resource type</span></span>

<span data-ttu-id="e9aba-104">Representa o plano de fundo de um objeto de intervalo.</span><span class="sxs-lookup"><span data-stu-id="e9aba-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="e9aba-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="e9aba-105">Methods</span></span>

| <span data-ttu-id="e9aba-106">Método</span><span class="sxs-lookup"><span data-stu-id="e9aba-106">Method</span></span>           | <span data-ttu-id="e9aba-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e9aba-107">Return Type</span></span>    |<span data-ttu-id="e9aba-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9aba-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e9aba-109">Get RangeFill</span><span class="sxs-lookup"><span data-stu-id="e9aba-109">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="e9aba-110">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="e9aba-110">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="e9aba-111">Leia as propriedades e os relacionamentos do objeto rangeFill.</span><span class="sxs-lookup"><span data-stu-id="e9aba-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="e9aba-112">Update</span><span class="sxs-lookup"><span data-stu-id="e9aba-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="e9aba-113">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="e9aba-113">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="e9aba-114">Atualize o objeto RangeFill.</span><span class="sxs-lookup"><span data-stu-id="e9aba-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="e9aba-115">Clear</span><span class="sxs-lookup"><span data-stu-id="e9aba-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="e9aba-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e9aba-116">None</span></span>|<span data-ttu-id="e9aba-117">Redefine o plano de fundo do intervalo.</span><span class="sxs-lookup"><span data-stu-id="e9aba-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="e9aba-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e9aba-118">Properties</span></span>
| <span data-ttu-id="e9aba-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9aba-119">Property</span></span>     | <span data-ttu-id="e9aba-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9aba-120">Type</span></span>   |<span data-ttu-id="e9aba-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9aba-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9aba-122">color</span><span class="sxs-lookup"><span data-stu-id="e9aba-122">color</span></span>|<span data-ttu-id="e9aba-123">string</span><span class="sxs-lookup"><span data-stu-id="e9aba-123">string</span></span>|<span data-ttu-id="e9aba-124">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="e9aba-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9aba-125">Relações</span><span class="sxs-lookup"><span data-stu-id="e9aba-125">Relationships</span></span>
<span data-ttu-id="e9aba-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e9aba-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e9aba-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e9aba-127">JSON representation</span></span>

<span data-ttu-id="e9aba-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e9aba-128">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFill"
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
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->