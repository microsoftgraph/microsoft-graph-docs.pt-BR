---
title: Tipo de recurso conditionalAccessDevices
description: Representa dispositivos no escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a42e6023ace493c5efb230ffd53eb9c4caee7d16
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440525"
---
# <a name="conditionalaccessdevices-resource-type"></a><span data-ttu-id="e2936-103">Tipo de recurso conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="e2936-103">conditionalAccessDevices resource type</span></span>

<span data-ttu-id="e2936-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2936-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2936-105">Representa dispositivos no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="e2936-105">Represents devices in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="e2936-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2936-106">Properties</span></span>

| <span data-ttu-id="e2936-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2936-107">Property</span></span>     | <span data-ttu-id="e2936-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2936-108">Type</span></span>        | <span data-ttu-id="e2936-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2936-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e2936-110">includeDevices</span><span class="sxs-lookup"><span data-stu-id="e2936-110">includeDevices</span></span> | <span data-ttu-id="e2936-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2936-111">String collection</span></span> | <span data-ttu-id="e2936-112">Estados no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="e2936-112">States in the scope of the policy.</span></span> <span data-ttu-id="e2936-113">`All` é o único valor permitido.</span><span class="sxs-lookup"><span data-stu-id="e2936-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="e2936-114">excludeDevices</span><span class="sxs-lookup"><span data-stu-id="e2936-114">excludeDevices</span></span> | <span data-ttu-id="e2936-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2936-115">String collection</span></span> | <span data-ttu-id="e2936-116">Estados excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="e2936-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="e2936-117">Valores possíveis: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="e2936-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |
| <span data-ttu-id="e2936-118">includeDeviceStates (preterido)</span><span class="sxs-lookup"><span data-stu-id="e2936-118">includeDeviceStates (deprecated)</span></span>| <span data-ttu-id="e2936-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2936-119">String collection</span></span> | <span data-ttu-id="e2936-120">Estados no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="e2936-120">States in the scope of the policy.</span></span> <span data-ttu-id="e2936-121">`All` é o único valor permitido.</span><span class="sxs-lookup"><span data-stu-id="e2936-121">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="e2936-122">excludeDeviceStates (preterido)</span><span class="sxs-lookup"><span data-stu-id="e2936-122">excludeDeviceStates (deprecated)</span></span>| <span data-ttu-id="e2936-123">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2936-123">String collection</span></span> | <span data-ttu-id="e2936-124">Estados excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="e2936-124">States excluded from the scope of the policy.</span></span> <span data-ttu-id="e2936-125">Valores possíveis: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="e2936-125">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e2936-126">Relações</span><span class="sxs-lookup"><span data-stu-id="e2936-126">Relationships</span></span>

<span data-ttu-id="e2936-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2936-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2936-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2936-128">JSON representation</span></span>

<span data-ttu-id="e2936-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2936-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeDevices",
    "excludeDevices"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDevices",
  "baseType": null
}-->

```json
{
  "includeDevices": [ "String" ],
  "excludeDevices": [ "String" ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessDevices resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


