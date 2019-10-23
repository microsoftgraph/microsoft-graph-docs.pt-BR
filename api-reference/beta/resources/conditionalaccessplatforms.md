---
title: tipo de recurso conditionalAccessPlatforms
description: Plataformas incluídas e excluídas do escopo da política.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9de4d82cac659e73c1b4a898d6de9017c8e3e830
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638502"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="a86c3-103">tipo de recurso conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="a86c3-103">conditionalAccessPlatforms resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a86c3-104">Plataformas incluídas e excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="a86c3-104">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="a86c3-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a86c3-105">Properties</span></span>

| <span data-ttu-id="a86c3-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a86c3-106">Property</span></span>     | <span data-ttu-id="a86c3-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a86c3-107">Type</span></span>        | <span data-ttu-id="a86c3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a86c3-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a86c3-109">includePlatforms</span><span class="sxs-lookup"><span data-stu-id="a86c3-109">includePlatforms</span></span>|<span data-ttu-id="a86c3-110">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a86c3-110">String collection</span></span>| <span data-ttu-id="a86c3-111">Os possíveis valores são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span><span class="sxs-lookup"><span data-stu-id="a86c3-111">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span></span>|
|<span data-ttu-id="a86c3-112">excludePlatforms</span><span class="sxs-lookup"><span data-stu-id="a86c3-112">excludePlatforms</span></span>|<span data-ttu-id="a86c3-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a86c3-113">String collection</span></span>| <span data-ttu-id="a86c3-114">Os valores possíveis são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="a86c3-114">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a86c3-115">Relações</span><span class="sxs-lookup"><span data-stu-id="a86c3-115">Relationships</span></span>

<span data-ttu-id="a86c3-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a86c3-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a86c3-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a86c3-117">JSON representation</span></span>

<span data-ttu-id="a86c3-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a86c3-118">The following is a JSON representation of the resource.</span></span>

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