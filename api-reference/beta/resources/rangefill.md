---
title: Tipo de recurso RangeFill
description: Representa o plano de fundo de um objeto de intervalo.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 8ceab66373331b6e144b69119d521a3e5ddccdc7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817756"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="45117-103">Tipo de recurso RangeFill</span><span class="sxs-lookup"><span data-stu-id="45117-103">RangeFill resource type</span></span>

> <span data-ttu-id="45117-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="45117-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45117-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="45117-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="45117-106">Representa o plano de fundo de um objeto de intervalo.</span><span class="sxs-lookup"><span data-stu-id="45117-106">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="45117-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="45117-107">Methods</span></span>

| <span data-ttu-id="45117-108">Método</span><span class="sxs-lookup"><span data-stu-id="45117-108">Method</span></span>           | <span data-ttu-id="45117-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="45117-109">Return Type</span></span>    |<span data-ttu-id="45117-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="45117-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="45117-111">Get RangeFill</span><span class="sxs-lookup"><span data-stu-id="45117-111">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="45117-112">RangeFill</span><span class="sxs-lookup"><span data-stu-id="45117-112">RangeFill</span></span>](rangefill.md) |<span data-ttu-id="45117-113">Leia as propriedades e os relacionamentos do objeto rangeFill.</span><span class="sxs-lookup"><span data-stu-id="45117-113">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="45117-114">Update</span><span class="sxs-lookup"><span data-stu-id="45117-114">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="45117-115">RangeFill</span><span class="sxs-lookup"><span data-stu-id="45117-115">RangeFill</span></span>](rangefill.md)   |<span data-ttu-id="45117-116">Atualize o objeto RangeFill.</span><span class="sxs-lookup"><span data-stu-id="45117-116">Update RangeFill object.</span></span> |
|[<span data-ttu-id="45117-117">Clear</span><span class="sxs-lookup"><span data-stu-id="45117-117">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="45117-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="45117-118">None</span></span>|<span data-ttu-id="45117-119">Redefine o plano de fundo do intervalo.</span><span class="sxs-lookup"><span data-stu-id="45117-119">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="45117-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45117-120">Properties</span></span>
| <span data-ttu-id="45117-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45117-121">Property</span></span>     | <span data-ttu-id="45117-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="45117-122">Type</span></span>   |<span data-ttu-id="45117-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="45117-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45117-124">color</span><span class="sxs-lookup"><span data-stu-id="45117-124">color</span></span>|<span data-ttu-id="45117-125">string</span><span class="sxs-lookup"><span data-stu-id="45117-125">string</span></span>|<span data-ttu-id="45117-126">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="45117-126">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="45117-127">Relações</span><span class="sxs-lookup"><span data-stu-id="45117-127">Relationships</span></span>
<span data-ttu-id="45117-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="45117-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="45117-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45117-129">JSON representation</span></span>

<span data-ttu-id="45117-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="45117-130">Here is a JSON representation of the resource.</span></span>

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
