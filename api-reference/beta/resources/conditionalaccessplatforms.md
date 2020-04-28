---
title: tipo de recurso conditionalAccessPlatforms
description: Plataformas incluídas e excluídas do escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 27cf8f2b6a022f4d5ca17d716b35b6f357d23471
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916786"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="94697-103">tipo de recurso conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="94697-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="94697-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94697-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94697-105">Plataformas incluídas e excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="94697-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="94697-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94697-106">Properties</span></span>

| <span data-ttu-id="94697-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94697-107">Property</span></span>     | <span data-ttu-id="94697-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="94697-108">Type</span></span>        | <span data-ttu-id="94697-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="94697-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="94697-110">includePlatforms</span><span class="sxs-lookup"><span data-stu-id="94697-110">includePlatforms</span></span>|<span data-ttu-id="94697-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="94697-111">String collection</span></span>| <span data-ttu-id="94697-112">Os possíveis valores são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span><span class="sxs-lookup"><span data-stu-id="94697-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span></span>|
|<span data-ttu-id="94697-113">excludePlatforms</span><span class="sxs-lookup"><span data-stu-id="94697-113">excludePlatforms</span></span>|<span data-ttu-id="94697-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="94697-114">String collection</span></span>| <span data-ttu-id="94697-115">Os valores possíveis são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="94697-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94697-116">Relações</span><span class="sxs-lookup"><span data-stu-id="94697-116">Relationships</span></span>

<span data-ttu-id="94697-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94697-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="94697-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94697-118">JSON representation</span></span>

<span data-ttu-id="94697-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94697-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessPlatforms",
  "baseType": null
}-->

```json
{
  "includePlatforms": ["String"],
  "excludePlatforms": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPlatforms resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->