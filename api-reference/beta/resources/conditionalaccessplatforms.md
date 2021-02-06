---
title: Tipo de recurso conditionalAccessPlatforms
description: Plataformas incluídas e excluídas do escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 69191885dd3e21aa0ab1f7d4266a33cfe1514e34
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132353"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="0853e-103">Tipo de recurso conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="0853e-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="0853e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0853e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0853e-105">Plataformas incluídas e excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="0853e-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="0853e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0853e-106">Properties</span></span>

| <span data-ttu-id="0853e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0853e-107">Property</span></span>     | <span data-ttu-id="0853e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0853e-108">Type</span></span>        | <span data-ttu-id="0853e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0853e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0853e-110">includePlatforms</span><span class="sxs-lookup"><span data-stu-id="0853e-110">includePlatforms</span></span>|<span data-ttu-id="0853e-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0853e-111">String collection</span></span>| <span data-ttu-id="0853e-112">Os possíveis valores são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span><span class="sxs-lookup"><span data-stu-id="0853e-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span></span>|
|<span data-ttu-id="0853e-113">excludePlatforms</span><span class="sxs-lookup"><span data-stu-id="0853e-113">excludePlatforms</span></span>|<span data-ttu-id="0853e-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0853e-114">String collection</span></span>| <span data-ttu-id="0853e-115">Os valores possíveis são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="0853e-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0853e-116">Relações</span><span class="sxs-lookup"><span data-stu-id="0853e-116">Relationships</span></span>

<span data-ttu-id="0853e-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0853e-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0853e-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0853e-118">JSON representation</span></span>

<span data-ttu-id="0853e-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0853e-119">The following is a JSON representation of the resource.</span></span>

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

