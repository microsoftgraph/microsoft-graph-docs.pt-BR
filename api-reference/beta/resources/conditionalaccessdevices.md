---
title: Tipo de recurso conditionalAccessDevices
description: Representa dispositivos no escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 94115e97c597bc34f03d843b8098f707ed39cd51
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761804"
---
# <a name="conditionalaccessdevices-resource-type"></a><span data-ttu-id="44cf6-103">Tipo de recurso conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="44cf6-103">conditionalAccessDevices resource type</span></span>

<span data-ttu-id="44cf6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44cf6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44cf6-105">Representa dispositivos no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="44cf6-105">Represents devices in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="44cf6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44cf6-106">Properties</span></span>

| <span data-ttu-id="44cf6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44cf6-107">Property</span></span>     | <span data-ttu-id="44cf6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="44cf6-108">Type</span></span>        | <span data-ttu-id="44cf6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="44cf6-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="44cf6-110">includeDevices</span><span class="sxs-lookup"><span data-stu-id="44cf6-110">includeDevices</span></span> | <span data-ttu-id="44cf6-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="44cf6-111">String collection</span></span> | <span data-ttu-id="44cf6-112">Estados no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="44cf6-112">States in the scope of the policy.</span></span> <span data-ttu-id="44cf6-113">`All` é o único valor permitido.</span><span class="sxs-lookup"><span data-stu-id="44cf6-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="44cf6-114">excludeDevices</span><span class="sxs-lookup"><span data-stu-id="44cf6-114">excludeDevices</span></span> | <span data-ttu-id="44cf6-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="44cf6-115">String collection</span></span> | <span data-ttu-id="44cf6-116">Estados excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="44cf6-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="44cf6-117">Valores possíveis: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="44cf6-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |
| <span data-ttu-id="44cf6-118">includeDeviceStates (preterido)</span><span class="sxs-lookup"><span data-stu-id="44cf6-118">includeDeviceStates (deprecated)</span></span>| <span data-ttu-id="44cf6-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="44cf6-119">String collection</span></span> | <span data-ttu-id="44cf6-120">Estados no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="44cf6-120">States in the scope of the policy.</span></span> <span data-ttu-id="44cf6-121">`All` é o único valor permitido.</span><span class="sxs-lookup"><span data-stu-id="44cf6-121">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="44cf6-122">excludeDeviceStates (preterido)</span><span class="sxs-lookup"><span data-stu-id="44cf6-122">excludeDeviceStates (deprecated)</span></span>| <span data-ttu-id="44cf6-123">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="44cf6-123">String collection</span></span> | <span data-ttu-id="44cf6-124">Estados excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="44cf6-124">States excluded from the scope of the policy.</span></span> <span data-ttu-id="44cf6-125">Valores possíveis: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="44cf6-125">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="44cf6-126">Relações</span><span class="sxs-lookup"><span data-stu-id="44cf6-126">Relationships</span></span>

<span data-ttu-id="44cf6-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="44cf6-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="44cf6-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44cf6-128">JSON representation</span></span>

<span data-ttu-id="44cf6-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="44cf6-129">The following is a JSON representation of the resource.</span></span>

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


