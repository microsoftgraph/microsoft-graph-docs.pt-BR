---
title: tipo de recurso conditionalAccessDeviceStates
description: Representa os Estados do dispositivo no escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 262657c015e4b3416baa9e6e533d1b8f76c1a536
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040068"
---
# <a name="conditionalaccessdevicestates-resource-type"></a><span data-ttu-id="5f398-103">tipo de recurso conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="5f398-103">conditionalAccessDeviceStates resource type</span></span>

<span data-ttu-id="5f398-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f398-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f398-105">Representa os Estados do dispositivo no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="5f398-105">Represents device states in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="5f398-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f398-106">Properties</span></span>

| <span data-ttu-id="5f398-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f398-107">Property</span></span>     | <span data-ttu-id="5f398-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f398-108">Type</span></span>        | <span data-ttu-id="5f398-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f398-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5f398-110">includeStates</span><span class="sxs-lookup"><span data-stu-id="5f398-110">includeStates</span></span> | <span data-ttu-id="5f398-111">Coleção String</span><span class="sxs-lookup"><span data-stu-id="5f398-111">String collection</span></span> | <span data-ttu-id="5f398-112">Estados no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="5f398-112">States in the scope of the policy.</span></span> <span data-ttu-id="5f398-113">`All` é o único valor permitido.</span><span class="sxs-lookup"><span data-stu-id="5f398-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="5f398-114">excludeStates</span><span class="sxs-lookup"><span data-stu-id="5f398-114">excludeStates</span></span> | <span data-ttu-id="5f398-115">Coleção String</span><span class="sxs-lookup"><span data-stu-id="5f398-115">String collection</span></span> | <span data-ttu-id="5f398-116">Estados excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="5f398-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="5f398-117">Valores possíveis: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="5f398-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5f398-118">Relações</span><span class="sxs-lookup"><span data-stu-id="5f398-118">Relationships</span></span>

<span data-ttu-id="5f398-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f398-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f398-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f398-120">JSON representation</span></span>

<span data-ttu-id="5f398-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f398-121">The following is a JSON representation of the resource.</span></span>

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

