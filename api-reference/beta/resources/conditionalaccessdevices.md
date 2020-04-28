---
title: tipo de recurso conditionalAccessDevices
description: Representa dispositivos no escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b10bef4904d443ca975f5f98834b3b2d1c72a7e7
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916813"
---
# <a name="conditionalaccessdevices-resource-type"></a><span data-ttu-id="f4bed-103">tipo de recurso conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="f4bed-103">conditionalAccessDevices resource type</span></span>

<span data-ttu-id="f4bed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4bed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4bed-105">Representa dispositivos no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="f4bed-105">Represents devices in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="f4bed-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4bed-106">Properties</span></span>

| <span data-ttu-id="f4bed-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4bed-107">Property</span></span>     | <span data-ttu-id="f4bed-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4bed-108">Type</span></span>        | <span data-ttu-id="f4bed-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4bed-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f4bed-110">includeDeviceStates</span><span class="sxs-lookup"><span data-stu-id="f4bed-110">includeDeviceStates</span></span> | <span data-ttu-id="f4bed-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4bed-111">String collection</span></span> | <span data-ttu-id="f4bed-112">Estados no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="f4bed-112">States in the scope of the policy.</span></span> <span data-ttu-id="f4bed-113">`All`é o único valor permitido.</span><span class="sxs-lookup"><span data-stu-id="f4bed-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="f4bed-114">excludeDeviceStates</span><span class="sxs-lookup"><span data-stu-id="f4bed-114">excludeDeviceStates</span></span> | <span data-ttu-id="f4bed-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4bed-115">String collection</span></span> | <span data-ttu-id="f4bed-116">Estados excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="f4bed-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="f4bed-117">Valores possíveis: `Compliant`, `DomainJoined`.</span><span class="sxs-lookup"><span data-stu-id="f4bed-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f4bed-118">Relações</span><span class="sxs-lookup"><span data-stu-id="f4bed-118">Relationships</span></span>

<span data-ttu-id="f4bed-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f4bed-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4bed-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4bed-120">JSON representation</span></span>

<span data-ttu-id="f4bed-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4bed-121">The following is a JSON representation of the resource.</span></span>

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
