---
title: Tipo de recurso conditionalAccessPlatforms
description: Plataformas incluídas e excluídas do escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b6dac42062d84746196caaa0a11c26af1549b555
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962480"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="a7c5a-103">Tipo de recurso conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="a7c5a-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="a7c5a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7c5a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a7c5a-105">Plataformas incluídas e excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="a7c5a-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="a7c5a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7c5a-106">Properties</span></span>

| <span data-ttu-id="a7c5a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7c5a-107">Property</span></span>     | <span data-ttu-id="a7c5a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7c5a-108">Type</span></span>        | <span data-ttu-id="a7c5a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7c5a-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a7c5a-110">includePlatforms</span><span class="sxs-lookup"><span data-stu-id="a7c5a-110">includePlatforms</span></span>|<span data-ttu-id="a7c5a-111">Coleção conditionalAccessDevicePlatform</span><span class="sxs-lookup"><span data-stu-id="a7c5a-111">conditionalAccessDevicePlatform collection</span></span>| <span data-ttu-id="a7c5a-112">Os valores possíveis são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a7c5a-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a7c5a-113">excludePlatforms</span><span class="sxs-lookup"><span data-stu-id="a7c5a-113">excludePlatforms</span></span>|<span data-ttu-id="a7c5a-114">Coleção conditionalAccessDevicePlatform</span><span class="sxs-lookup"><span data-stu-id="a7c5a-114">conditionalAccessDevicePlatform collection</span></span>| <span data-ttu-id="a7c5a-115">Os valores possíveis são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a7c5a-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7c5a-116">Relações</span><span class="sxs-lookup"><span data-stu-id="a7c5a-116">Relationships</span></span>

<span data-ttu-id="a7c5a-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7c5a-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7c5a-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7c5a-118">JSON representation</span></span>

<span data-ttu-id="a7c5a-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a7c5a-119">The following is a JSON representation of the resource.</span></span>

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

