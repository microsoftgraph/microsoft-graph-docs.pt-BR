---
title: tipo de recurso conditionalAccessDeviceStates
description: Representa os Estados do dispositivo no escopo da política.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 03981fc5be0388e8146c163ab4500eae87d65704
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413499"
---
# <a name="conditionalaccessdevicestates-resource-type"></a><span data-ttu-id="dcac8-103">tipo de recurso conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="dcac8-103">conditionalAccessDeviceStates resource type</span></span>

<span data-ttu-id="dcac8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcac8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcac8-105">Representa os Estados do dispositivo no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="dcac8-105">Represents device states in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="dcac8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dcac8-106">Properties</span></span>

| <span data-ttu-id="dcac8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dcac8-107">Property</span></span>     | <span data-ttu-id="dcac8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="dcac8-108">Type</span></span>        | <span data-ttu-id="dcac8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcac8-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="dcac8-110">includeStates</span><span class="sxs-lookup"><span data-stu-id="dcac8-110">includeStates</span></span> | <span data-ttu-id="dcac8-111">Coleção String</span><span class="sxs-lookup"><span data-stu-id="dcac8-111">String collection</span></span> | <span data-ttu-id="dcac8-112">Estados no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="dcac8-112">States in the scope of the policy.</span></span> <span data-ttu-id="dcac8-113">`All`é o único valor permitido.</span><span class="sxs-lookup"><span data-stu-id="dcac8-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="dcac8-114">excludeStates</span><span class="sxs-lookup"><span data-stu-id="dcac8-114">excludeStates</span></span> | <span data-ttu-id="dcac8-115">Coleção String</span><span class="sxs-lookup"><span data-stu-id="dcac8-115">String collection</span></span> | <span data-ttu-id="dcac8-116">Estados excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="dcac8-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="dcac8-117">Valores possíveis: `Compliant`, `DomainJoined`.</span><span class="sxs-lookup"><span data-stu-id="dcac8-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dcac8-118">Relações</span><span class="sxs-lookup"><span data-stu-id="dcac8-118">Relationships</span></span>

<span data-ttu-id="dcac8-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dcac8-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dcac8-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dcac8-120">JSON representation</span></span>

<span data-ttu-id="dcac8-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dcac8-121">The following is a JSON representation of the resource.</span></span>

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