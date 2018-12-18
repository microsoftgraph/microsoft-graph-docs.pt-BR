---
title: Tipo de recurso RangeFill
description: Representa o plano de fundo de um objeto de intervalo.
author: lumine2008
ms.openlocfilehash: 21d40b1ec65ad49241af30912c3c05e114c7008d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323706"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="47eeb-103">Tipo de recurso RangeFill</span><span class="sxs-lookup"><span data-stu-id="47eeb-103">RangeFill resource type</span></span>

> <span data-ttu-id="47eeb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="47eeb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47eeb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="47eeb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="47eeb-106">Representa o plano de fundo de um objeto de intervalo.</span><span class="sxs-lookup"><span data-stu-id="47eeb-106">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="47eeb-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="47eeb-107">Methods</span></span>

| <span data-ttu-id="47eeb-108">Método</span><span class="sxs-lookup"><span data-stu-id="47eeb-108">Method</span></span>           | <span data-ttu-id="47eeb-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="47eeb-109">Return Type</span></span>    |<span data-ttu-id="47eeb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="47eeb-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="47eeb-111">Get RangeFill</span><span class="sxs-lookup"><span data-stu-id="47eeb-111">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="47eeb-112">RangeFill</span><span class="sxs-lookup"><span data-stu-id="47eeb-112">RangeFill</span></span>](rangefill.md) |<span data-ttu-id="47eeb-113">Leia as propriedades e os relacionamentos do objeto rangeFill.</span><span class="sxs-lookup"><span data-stu-id="47eeb-113">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="47eeb-114">Update</span><span class="sxs-lookup"><span data-stu-id="47eeb-114">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="47eeb-115">RangeFill</span><span class="sxs-lookup"><span data-stu-id="47eeb-115">RangeFill</span></span>](rangefill.md)   |<span data-ttu-id="47eeb-116">Atualize o objeto RangeFill.</span><span class="sxs-lookup"><span data-stu-id="47eeb-116">Update RangeFill object.</span></span> |
|[<span data-ttu-id="47eeb-117">Clear</span><span class="sxs-lookup"><span data-stu-id="47eeb-117">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="47eeb-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47eeb-118">None</span></span>|<span data-ttu-id="47eeb-119">Redefine o plano de fundo do intervalo.</span><span class="sxs-lookup"><span data-stu-id="47eeb-119">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="47eeb-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47eeb-120">Properties</span></span>
| <span data-ttu-id="47eeb-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47eeb-121">Property</span></span>     | <span data-ttu-id="47eeb-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="47eeb-122">Type</span></span>   |<span data-ttu-id="47eeb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="47eeb-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47eeb-124">color</span><span class="sxs-lookup"><span data-stu-id="47eeb-124">color</span></span>|<span data-ttu-id="47eeb-125">string</span><span class="sxs-lookup"><span data-stu-id="47eeb-125">string</span></span>|<span data-ttu-id="47eeb-126">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="47eeb-126">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="47eeb-127">Relações</span><span class="sxs-lookup"><span data-stu-id="47eeb-127">Relationships</span></span>
<span data-ttu-id="47eeb-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47eeb-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="47eeb-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47eeb-129">JSON representation</span></span>

<span data-ttu-id="47eeb-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47eeb-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFill"
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