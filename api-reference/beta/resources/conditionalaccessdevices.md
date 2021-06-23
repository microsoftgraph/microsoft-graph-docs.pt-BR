---
title: Tipo de recurso conditionalAccessDevices
description: Representa dispositivos no escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: cbb542420228a4a383dea4e165323fbb6e8abb17
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082353"
---
# <a name="conditionalaccessdevices-resource-type"></a><span data-ttu-id="495d6-103">Tipo de recurso conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="495d6-103">conditionalAccessDevices resource type</span></span>

<span data-ttu-id="495d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="495d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="495d6-105">Representa dispositivos no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="495d6-105">Represents devices in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="495d6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="495d6-106">Properties</span></span>

| <span data-ttu-id="495d6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="495d6-107">Property</span></span>     | <span data-ttu-id="495d6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="495d6-108">Type</span></span>        | <span data-ttu-id="495d6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="495d6-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="495d6-110">includeDevices</span><span class="sxs-lookup"><span data-stu-id="495d6-110">includeDevices</span></span> | <span data-ttu-id="495d6-111">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="495d6-111">String collection</span></span> | <span data-ttu-id="495d6-112">Estados no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="495d6-112">States in the scope of the policy.</span></span> <span data-ttu-id="495d6-113">`All` é o único valor permitido.</span><span class="sxs-lookup"><span data-stu-id="495d6-113">`All` is the only allowed value.</span></span> <span data-ttu-id="495d6-114">Não será possível definir *se deviceFIlter* estiver definido.</span><span class="sxs-lookup"><span data-stu-id="495d6-114">Cannot be set if *deviceFIlter* is set.</span></span> |
| <span data-ttu-id="495d6-115">excludeDevices</span><span class="sxs-lookup"><span data-stu-id="495d6-115">excludeDevices</span></span> | <span data-ttu-id="495d6-116">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="495d6-116">String collection</span></span> | <span data-ttu-id="495d6-117">Estados excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="495d6-117">States excluded from the scope of the policy.</span></span> <span data-ttu-id="495d6-118">Valores possíveis: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="495d6-118">Possible values: `Compliant`, `DomainJoined`.</span></span> <span data-ttu-id="495d6-119">Não será possível definir **se deviceFIlter** estiver definido.</span><span class="sxs-lookup"><span data-stu-id="495d6-119">Cannot be set if **deviceFIlter** is set.</span></span> |
| <span data-ttu-id="495d6-120">deviceFilter</span><span class="sxs-lookup"><span data-stu-id="495d6-120">deviceFilter</span></span> | [<span data-ttu-id="495d6-121">conditionalAccessFilter</span><span class="sxs-lookup"><span data-stu-id="495d6-121">conditionalAccessFilter</span></span>](conditionalaccessfilter.md) | <span data-ttu-id="495d6-122">Filtrar definindo a regra de sintaxe de dispositivo dinâmico para incluir/excluir dispositivos.</span><span class="sxs-lookup"><span data-stu-id="495d6-122">Filter defining the dynamic-device-syntax rule to include/exclude devices.</span></span> <span data-ttu-id="495d6-123">Um filtro pode usar propriedades de dispositivo (como atributos de extensão) para incluí-las/excluir.</span><span class="sxs-lookup"><span data-stu-id="495d6-123">A filter can use device properties (such as extension attributes) to include/exclude them.</span></span> <span data-ttu-id="495d6-124">Não será possível definir **se includeDevices** ou **excludeDevices** estiver definido.</span><span class="sxs-lookup"><span data-stu-id="495d6-124">Cannot be set if **includeDevices** or **excludeDevices** is set.</span></span> |
| <span data-ttu-id="495d6-125">includeDeviceStates (preterido)</span><span class="sxs-lookup"><span data-stu-id="495d6-125">includeDeviceStates (deprecated)</span></span>| <span data-ttu-id="495d6-126">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="495d6-126">String collection</span></span> | <span data-ttu-id="495d6-127">Estados no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="495d6-127">States in the scope of the policy.</span></span> <span data-ttu-id="495d6-128">`All` é o único valor permitido.</span><span class="sxs-lookup"><span data-stu-id="495d6-128">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="495d6-129">excludeDeviceStates (preterido)</span><span class="sxs-lookup"><span data-stu-id="495d6-129">excludeDeviceStates (deprecated)</span></span>| <span data-ttu-id="495d6-130">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="495d6-130">String collection</span></span> | <span data-ttu-id="495d6-131">Estados excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="495d6-131">States excluded from the scope of the policy.</span></span> <span data-ttu-id="495d6-132">Valores possíveis: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="495d6-132">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="495d6-133">Relações</span><span class="sxs-lookup"><span data-stu-id="495d6-133">Relationships</span></span>

<span data-ttu-id="495d6-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="495d6-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="495d6-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="495d6-135">JSON representation</span></span>

<span data-ttu-id="495d6-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="495d6-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeDevices",
    "excludeDevices",
    "deviceFilter"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDevices",
  "baseType": null
}-->

```json
{
  "includeDevices": [ "String" ],
  "excludeDevices": [ "String" ],
  "deviceFilter": {"@odata.type": "microsoft.graph.conditionalAccessFilter"}
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


