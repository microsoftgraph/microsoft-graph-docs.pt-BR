---
title: Tipo de recurso conditionalAccessPlatforms
description: Plataformas incluídas e excluídas do escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 71c8b38b59d30ce1e8e1fa1c7668c41a5d2288c2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945701"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="86e50-103">Tipo de recurso conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="86e50-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="86e50-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86e50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86e50-105">Plataformas incluídas e excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="86e50-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="86e50-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86e50-106">Properties</span></span>

| <span data-ttu-id="86e50-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86e50-107">Property</span></span>     | <span data-ttu-id="86e50-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="86e50-108">Type</span></span>        | <span data-ttu-id="86e50-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="86e50-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="86e50-110">includePlatforms</span><span class="sxs-lookup"><span data-stu-id="86e50-110">includePlatforms</span></span>|<span data-ttu-id="86e50-111">Coleção conditionalAccessDevicePlatform</span><span class="sxs-lookup"><span data-stu-id="86e50-111">conditionalAccessDevicePlatform collection</span></span>| <span data-ttu-id="86e50-112">Os valores possíveis são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="86e50-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="86e50-113">excludePlatforms</span><span class="sxs-lookup"><span data-stu-id="86e50-113">excludePlatforms</span></span>|<span data-ttu-id="86e50-114">Coleção conditionalAccessDevicePlatform</span><span class="sxs-lookup"><span data-stu-id="86e50-114">conditionalAccessDevicePlatform collection</span></span>| <span data-ttu-id="86e50-115">Os valores possíveis são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="86e50-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86e50-116">Relações</span><span class="sxs-lookup"><span data-stu-id="86e50-116">Relationships</span></span>

<span data-ttu-id="86e50-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="86e50-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="86e50-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86e50-118">JSON representation</span></span>

<span data-ttu-id="86e50-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86e50-119">The following is a JSON representation of the resource.</span></span>

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

