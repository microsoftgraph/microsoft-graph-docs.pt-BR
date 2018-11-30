---
title: Tipo de recurso RangeFill
description: Representa o plano de fundo de um objeto de intervalo.
ms.openlocfilehash: 11806d95900c6e4ea1d4bf6ce4f4800bf5f6f66b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039976"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="ff1c0-103">Tipo de recurso RangeFill</span><span class="sxs-lookup"><span data-stu-id="ff1c0-103">RangeFill resource type</span></span>

> <span data-ttu-id="ff1c0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ff1c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff1c0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ff1c0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff1c0-106">Representa o plano de fundo de um objeto de intervalo.</span><span class="sxs-lookup"><span data-stu-id="ff1c0-106">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="ff1c0-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ff1c0-107">Methods</span></span>

| <span data-ttu-id="ff1c0-108">Método</span><span class="sxs-lookup"><span data-stu-id="ff1c0-108">Method</span></span>           | <span data-ttu-id="ff1c0-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ff1c0-109">Return Type</span></span>    |<span data-ttu-id="ff1c0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff1c0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff1c0-111">Get RangeFill</span><span class="sxs-lookup"><span data-stu-id="ff1c0-111">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="ff1c0-112">RangeFill</span><span class="sxs-lookup"><span data-stu-id="ff1c0-112">RangeFill</span></span>](rangefill.md) |<span data-ttu-id="ff1c0-113">Leia as propriedades e os relacionamentos do objeto rangeFill.</span><span class="sxs-lookup"><span data-stu-id="ff1c0-113">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="ff1c0-114">Update</span><span class="sxs-lookup"><span data-stu-id="ff1c0-114">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="ff1c0-115">RangeFill</span><span class="sxs-lookup"><span data-stu-id="ff1c0-115">RangeFill</span></span>](rangefill.md)   |<span data-ttu-id="ff1c0-116">Atualize o objeto RangeFill.</span><span class="sxs-lookup"><span data-stu-id="ff1c0-116">Update RangeFill object.</span></span> |
|[<span data-ttu-id="ff1c0-117">Clear</span><span class="sxs-lookup"><span data-stu-id="ff1c0-117">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="ff1c0-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff1c0-118">None</span></span>|<span data-ttu-id="ff1c0-119">Redefine o plano de fundo do intervalo.</span><span class="sxs-lookup"><span data-stu-id="ff1c0-119">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff1c0-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff1c0-120">Properties</span></span>
| <span data-ttu-id="ff1c0-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff1c0-121">Property</span></span>     | <span data-ttu-id="ff1c0-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff1c0-122">Type</span></span>   |<span data-ttu-id="ff1c0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff1c0-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff1c0-124">color</span><span class="sxs-lookup"><span data-stu-id="ff1c0-124">color</span></span>|<span data-ttu-id="ff1c0-125">string</span><span class="sxs-lookup"><span data-stu-id="ff1c0-125">string</span></span>|<span data-ttu-id="ff1c0-126">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="ff1c0-126">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff1c0-127">Relações</span><span class="sxs-lookup"><span data-stu-id="ff1c0-127">Relationships</span></span>
<span data-ttu-id="ff1c0-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff1c0-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ff1c0-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff1c0-129">JSON representation</span></span>

<span data-ttu-id="ff1c0-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff1c0-130">Here is a JSON representation of the resource.</span></span>

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