---
title: tipo de recurso conditionalAccessPlatforms
description: Plataformas incluídas e excluídas do escopo da política.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2612b352f512d1177bc9137603b6ecda1ad96f66
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507531"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="b2678-103">tipo de recurso conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="b2678-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="b2678-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b2678-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2678-105">Plataformas incluídas e excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="b2678-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="b2678-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2678-106">Properties</span></span>

| <span data-ttu-id="b2678-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2678-107">Property</span></span>     | <span data-ttu-id="b2678-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2678-108">Type</span></span>        | <span data-ttu-id="b2678-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2678-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b2678-110">includePlatforms</span><span class="sxs-lookup"><span data-stu-id="b2678-110">includePlatforms</span></span>|<span data-ttu-id="b2678-111">String collection</span><span class="sxs-lookup"><span data-stu-id="b2678-111">String collection</span></span>| <span data-ttu-id="b2678-112">Os possíveis valores são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span><span class="sxs-lookup"><span data-stu-id="b2678-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span></span>|
|<span data-ttu-id="b2678-113">excludePlatforms</span><span class="sxs-lookup"><span data-stu-id="b2678-113">excludePlatforms</span></span>|<span data-ttu-id="b2678-114">String collection</span><span class="sxs-lookup"><span data-stu-id="b2678-114">String collection</span></span>| <span data-ttu-id="b2678-115">Os valores possíveis são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="b2678-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2678-116">Relações</span><span class="sxs-lookup"><span data-stu-id="b2678-116">Relationships</span></span>

<span data-ttu-id="b2678-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2678-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2678-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2678-118">JSON representation</span></span>

<span data-ttu-id="b2678-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b2678-119">The following is a JSON representation of the resource.</span></span>

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