---
title: tipo de recurso conditionalAccessDeviceStates
description: Representa os Estados do dispositivo no escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c23406f63ae94a494e972d4063277c277d655423
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916798"
---
# <a name="conditionalaccessdevicestates-resource-type"></a><span data-ttu-id="6a924-103">tipo de recurso conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="6a924-103">conditionalAccessDeviceStates resource type</span></span>

<span data-ttu-id="6a924-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a924-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a924-105">Representa os Estados do dispositivo no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="6a924-105">Represents device states in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="6a924-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a924-106">Properties</span></span>

| <span data-ttu-id="6a924-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a924-107">Property</span></span>     | <span data-ttu-id="6a924-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a924-108">Type</span></span>        | <span data-ttu-id="6a924-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a924-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6a924-110">includeStates</span><span class="sxs-lookup"><span data-stu-id="6a924-110">includeStates</span></span> | <span data-ttu-id="6a924-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a924-111">String collection</span></span> | <span data-ttu-id="6a924-112">Estados no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="6a924-112">States in the scope of the policy.</span></span> <span data-ttu-id="6a924-113">`All`é o único valor permitido.</span><span class="sxs-lookup"><span data-stu-id="6a924-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="6a924-114">excludeStates</span><span class="sxs-lookup"><span data-stu-id="6a924-114">excludeStates</span></span> | <span data-ttu-id="6a924-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a924-115">String collection</span></span> | <span data-ttu-id="6a924-116">Estados excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="6a924-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="6a924-117">Valores possíveis: `Compliant`, `DomainJoined`.</span><span class="sxs-lookup"><span data-stu-id="6a924-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6a924-118">Relações</span><span class="sxs-lookup"><span data-stu-id="6a924-118">Relationships</span></span>

<span data-ttu-id="6a924-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a924-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a924-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a924-120">JSON representation</span></span>

<span data-ttu-id="6a924-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a924-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeStates",
    "excludeStates"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDeviceStates",
  "baseType": null
}-->

```json
{
  "includeStates": [ "String" ],
  "excludeStates": [ "String" ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessDeviceStates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->