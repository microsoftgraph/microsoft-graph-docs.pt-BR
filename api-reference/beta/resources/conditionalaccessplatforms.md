---
title: tipo de recurso conditionalAccessPlatforms
description: Plataformas incluídas e excluídas do escopo da política.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5907e7162093b7d0d9fb796f61fc0cf110350417
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413350"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="d4e2b-103">tipo de recurso conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="d4e2b-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="d4e2b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4e2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4e2b-105">Plataformas incluídas e excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="d4e2b-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="d4e2b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4e2b-106">Properties</span></span>

| <span data-ttu-id="d4e2b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4e2b-107">Property</span></span>     | <span data-ttu-id="d4e2b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4e2b-108">Type</span></span>        | <span data-ttu-id="d4e2b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4e2b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d4e2b-110">includePlatforms</span><span class="sxs-lookup"><span data-stu-id="d4e2b-110">includePlatforms</span></span>|<span data-ttu-id="d4e2b-111">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d4e2b-111">String collection</span></span>| <span data-ttu-id="d4e2b-112">Os possíveis valores são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span><span class="sxs-lookup"><span data-stu-id="d4e2b-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span></span>|
|<span data-ttu-id="d4e2b-113">excludePlatforms</span><span class="sxs-lookup"><span data-stu-id="d4e2b-113">excludePlatforms</span></span>|<span data-ttu-id="d4e2b-114">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d4e2b-114">String collection</span></span>| <span data-ttu-id="d4e2b-115">Os valores possíveis são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="d4e2b-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4e2b-116">Relações</span><span class="sxs-lookup"><span data-stu-id="d4e2b-116">Relationships</span></span>

<span data-ttu-id="d4e2b-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4e2b-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4e2b-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4e2b-118">JSON representation</span></span>

<span data-ttu-id="d4e2b-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4e2b-119">The following is a JSON representation of the resource.</span></span>

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