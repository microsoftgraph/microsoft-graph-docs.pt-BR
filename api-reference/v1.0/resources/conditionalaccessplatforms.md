---
title: tipo de recurso conditionalAccessPlatforms
description: Plataformas incluídas e excluídas do escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 88d40fa1557102bc04ef9a46bba93a50097d66cd
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384400"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="93210-103">tipo de recurso conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="93210-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="93210-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93210-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93210-105">Plataformas incluídas e excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="93210-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="93210-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93210-106">Properties</span></span>

| <span data-ttu-id="93210-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93210-107">Property</span></span>     | <span data-ttu-id="93210-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="93210-108">Type</span></span>        | <span data-ttu-id="93210-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="93210-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="93210-110">includePlatforms</span><span class="sxs-lookup"><span data-stu-id="93210-110">includePlatforms</span></span>|<span data-ttu-id="93210-111">String collection</span><span class="sxs-lookup"><span data-stu-id="93210-111">String collection</span></span>| <span data-ttu-id="93210-112">Os valores possíveis são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="93210-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="93210-113">excludePlatforms</span><span class="sxs-lookup"><span data-stu-id="93210-113">excludePlatforms</span></span>|<span data-ttu-id="93210-114">String collection</span><span class="sxs-lookup"><span data-stu-id="93210-114">String collection</span></span>| <span data-ttu-id="93210-115">Os possíveis valores são: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="93210-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93210-116">Relações</span><span class="sxs-lookup"><span data-stu-id="93210-116">Relationships</span></span>

<span data-ttu-id="93210-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93210-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="93210-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93210-118">JSON representation</span></span>

<span data-ttu-id="93210-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93210-119">The following is a JSON representation of the resource.</span></span>

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
