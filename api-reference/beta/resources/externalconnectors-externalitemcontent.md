---
title: Tipo de recurso externalItemContent
description: O conteúdo de um item indexado por meio de Pesquisa da Microsoft conexão.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: d895d0056da71ea065dbc62d08c9deda054a6f29
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467600"
---
# <a name="externalitemcontent-resource-type"></a><span data-ttu-id="f0627-103">Tipo de recurso externalItemContent</span><span class="sxs-lookup"><span data-stu-id="f0627-103">externalItemContent resource type</span></span>

<span data-ttu-id="f0627-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="f0627-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0627-105">O conteúdo de [um externalItem](externalconnectors-externalitem.md) indexado por meio de uma conexão Pesquisa da Microsoft [.](externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="f0627-105">The content of an [externalItem](externalconnectors-externalitem.md) indexed via a Microsoft Search [connection](externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f0627-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0627-106">Properties</span></span>

| <span data-ttu-id="f0627-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0627-107">Property</span></span> | <span data-ttu-id="f0627-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0627-108">Type</span></span>   | <span data-ttu-id="f0627-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0627-109">Description</span></span>                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| <span data-ttu-id="f0627-110">valor</span><span class="sxs-lookup"><span data-stu-id="f0627-110">value</span></span>    | <span data-ttu-id="f0627-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0627-111">String</span></span> | <span data-ttu-id="f0627-112">O conteúdo do externalItem.</span><span class="sxs-lookup"><span data-stu-id="f0627-112">The content for the externalItem.</span></span> <span data-ttu-id="f0627-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0627-113">Required.</span></span>                                                 |
| <span data-ttu-id="f0627-114">tipo</span><span class="sxs-lookup"><span data-stu-id="f0627-114">type</span></span>     | <span data-ttu-id="f0627-115">String</span><span class="sxs-lookup"><span data-stu-id="f0627-115">String</span></span> | <span data-ttu-id="f0627-116">O tipo de conteúdo na propriedade value.</span><span class="sxs-lookup"><span data-stu-id="f0627-116">The type of content in the value property.</span></span> <span data-ttu-id="f0627-117">Os valores possíveis são: `text` e `html`.</span><span class="sxs-lookup"><span data-stu-id="f0627-117">Possible values are `text` and `html`.</span></span> <span data-ttu-id="f0627-118">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0627-118">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f0627-119">Relações</span><span class="sxs-lookup"><span data-stu-id="f0627-119">Relationships</span></span>

<span data-ttu-id="f0627-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0627-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0627-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0627-121">JSON representation</span></span>

<span data-ttu-id="f0627-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0627-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalItemContent"
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