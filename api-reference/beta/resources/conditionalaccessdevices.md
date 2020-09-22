---
title: tipo de recurso conditionalAccessDevices
description: Representa dispositivos no escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f0610fb376b265a261b8a88ab4181dd89bb9f6c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040067"
---
# <a name="conditionalaccessdevices-resource-type"></a><span data-ttu-id="a8fb3-103">tipo de recurso conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="a8fb3-103">conditionalAccessDevices resource type</span></span>

<span data-ttu-id="a8fb3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8fb3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8fb3-105">Representa dispositivos no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="a8fb3-105">Represents devices in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="a8fb3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8fb3-106">Properties</span></span>

| <span data-ttu-id="a8fb3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8fb3-107">Property</span></span>     | <span data-ttu-id="a8fb3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8fb3-108">Type</span></span>        | <span data-ttu-id="a8fb3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8fb3-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a8fb3-110">includeDeviceStates</span><span class="sxs-lookup"><span data-stu-id="a8fb3-110">includeDeviceStates</span></span> | <span data-ttu-id="a8fb3-111">Coleção String</span><span class="sxs-lookup"><span data-stu-id="a8fb3-111">String collection</span></span> | <span data-ttu-id="a8fb3-112">Estados no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="a8fb3-112">States in the scope of the policy.</span></span> <span data-ttu-id="a8fb3-113">`All` é o único valor permitido.</span><span class="sxs-lookup"><span data-stu-id="a8fb3-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="a8fb3-114">excludeDeviceStates</span><span class="sxs-lookup"><span data-stu-id="a8fb3-114">excludeDeviceStates</span></span> | <span data-ttu-id="a8fb3-115">Coleção String</span><span class="sxs-lookup"><span data-stu-id="a8fb3-115">String collection</span></span> | <span data-ttu-id="a8fb3-116">Estados excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="a8fb3-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="a8fb3-117">Valores possíveis: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="a8fb3-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a8fb3-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a8fb3-118">Relationships</span></span>

<span data-ttu-id="a8fb3-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8fb3-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8fb3-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8fb3-120">JSON representation</span></span>

<span data-ttu-id="a8fb3-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8fb3-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeDeviceStates",
    "excludeDeviceStates"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDevices",
  "baseType": null
}-->

```json
{
  "includeDeviceStates": [ "String" ],
  "excludeDeviceStates": [ "String" ]
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


