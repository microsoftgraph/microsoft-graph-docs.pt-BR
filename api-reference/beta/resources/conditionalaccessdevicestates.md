---
title: tipo de recurso conditionalAccessDeviceStates
description: Representa os Estados do dispositivo no escopo da política.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ff61b1d9713a0da322d01e3c302ebefc98dbee46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507552"
---
# <a name="conditionalaccessdevicestates-resource-type"></a><span data-ttu-id="5f132-103">tipo de recurso conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="5f132-103">conditionalAccessDeviceStates resource type</span></span>

<span data-ttu-id="5f132-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5f132-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f132-105">Representa os Estados do dispositivo no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="5f132-105">Represents device states in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="5f132-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f132-106">Properties</span></span>

| <span data-ttu-id="5f132-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f132-107">Property</span></span>     | <span data-ttu-id="5f132-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f132-108">Type</span></span>        | <span data-ttu-id="5f132-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f132-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5f132-110">includeStates</span><span class="sxs-lookup"><span data-stu-id="5f132-110">includeStates</span></span> | <span data-ttu-id="5f132-111">String collection</span><span class="sxs-lookup"><span data-stu-id="5f132-111">String collection</span></span> | <span data-ttu-id="5f132-112">Estados no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="5f132-112">States in the scope of the policy.</span></span> <span data-ttu-id="5f132-113">`All`é o único valor permitido.</span><span class="sxs-lookup"><span data-stu-id="5f132-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="5f132-114">excludeStates</span><span class="sxs-lookup"><span data-stu-id="5f132-114">excludeStates</span></span> | <span data-ttu-id="5f132-115">String collection</span><span class="sxs-lookup"><span data-stu-id="5f132-115">String collection</span></span> | <span data-ttu-id="5f132-116">Estados excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="5f132-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="5f132-117">Valores possíveis: `Compliant`, `DomainJoined`.</span><span class="sxs-lookup"><span data-stu-id="5f132-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5f132-118">Relações</span><span class="sxs-lookup"><span data-stu-id="5f132-118">Relationships</span></span>

<span data-ttu-id="5f132-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f132-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f132-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f132-120">JSON representation</span></span>

<span data-ttu-id="5f132-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f132-121">The following is a JSON representation of the resource.</span></span>

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