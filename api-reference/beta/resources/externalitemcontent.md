---
title: Tipo de recurso externalItemContent
description: O conteúdo de um item indexado por meio de Pesquisa da Microsoft conexão.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 036b2e2d4081160680b7f5471bd2707ee503bc4a
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366538"
---
# <a name="externalitemcontent-resource-type"></a><span data-ttu-id="feb44-103">Tipo de recurso externalItemContent</span><span class="sxs-lookup"><span data-stu-id="feb44-103">externalItemContent resource type</span></span>

<span data-ttu-id="feb44-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="feb44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="feb44-105">O conteúdo de [um externalItem](externalitem.md) indexado por meio de uma conexão Pesquisa da Microsoft [.](externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="feb44-105">The content of an [externalItem](externalitem.md) indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="feb44-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="feb44-106">Properties</span></span>

| <span data-ttu-id="feb44-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="feb44-107">Property</span></span> | <span data-ttu-id="feb44-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="feb44-108">Type</span></span>   | <span data-ttu-id="feb44-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="feb44-109">Description</span></span>                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| <span data-ttu-id="feb44-110">valor</span><span class="sxs-lookup"><span data-stu-id="feb44-110">value</span></span>    | <span data-ttu-id="feb44-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="feb44-111">String</span></span> | <span data-ttu-id="feb44-112">O conteúdo do externalItem.</span><span class="sxs-lookup"><span data-stu-id="feb44-112">The content for the externalItem.</span></span> <span data-ttu-id="feb44-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="feb44-113">Required.</span></span>                                                 |
| <span data-ttu-id="feb44-114">tipo</span><span class="sxs-lookup"><span data-stu-id="feb44-114">type</span></span>     | <span data-ttu-id="feb44-115">String</span><span class="sxs-lookup"><span data-stu-id="feb44-115">String</span></span> | <span data-ttu-id="feb44-116">O tipo de conteúdo na propriedade value.</span><span class="sxs-lookup"><span data-stu-id="feb44-116">The type of content in the value property.</span></span> <span data-ttu-id="feb44-117">Os valores possíveis são: `text` e `html`.</span><span class="sxs-lookup"><span data-stu-id="feb44-117">Possible values are `text` and `html`.</span></span> <span data-ttu-id="feb44-118">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="feb44-118">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="feb44-119">Relações</span><span class="sxs-lookup"><span data-stu-id="feb44-119">Relationships</span></span>

<span data-ttu-id="feb44-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="feb44-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="feb44-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="feb44-121">JSON representation</span></span>

<span data-ttu-id="feb44-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="feb44-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItemContent"
}-->

```json
{
  "value": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalItemContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->


