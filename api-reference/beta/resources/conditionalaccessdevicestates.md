---
title: tipo de recurso conditionalAccessDeviceStates
description: Representa os Estados do dispositivo no escopo da política.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 822f819cd8e9ef0f93279c67b94972a1e9fb7929
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638579"
---
# <a name="conditionalaccessdevicestates-resource-type"></a><span data-ttu-id="ce462-103">tipo de recurso conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="ce462-103">conditionalAccessDeviceStates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce462-104">Representa os Estados do dispositivo no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="ce462-104">Represents device states in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="ce462-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce462-105">Properties</span></span>

| <span data-ttu-id="ce462-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce462-106">Property</span></span>     | <span data-ttu-id="ce462-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce462-107">Type</span></span>        | <span data-ttu-id="ce462-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce462-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ce462-109">includeStates</span><span class="sxs-lookup"><span data-stu-id="ce462-109">includeStates</span></span> | <span data-ttu-id="ce462-110">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce462-110">String collection</span></span> | <span data-ttu-id="ce462-111">Estados no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="ce462-111">States in the scope of the policy.</span></span> <span data-ttu-id="ce462-112">`All`é o único valor permitido.</span><span class="sxs-lookup"><span data-stu-id="ce462-112">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="ce462-113">excludeStates</span><span class="sxs-lookup"><span data-stu-id="ce462-113">excludeStates</span></span> | <span data-ttu-id="ce462-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce462-114">String collection</span></span> | <span data-ttu-id="ce462-115">Estados excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="ce462-115">States excluded from the scope of the policy.</span></span> <span data-ttu-id="ce462-116">Valores possíveis: `Compliant`, `DomainJoined`.</span><span class="sxs-lookup"><span data-stu-id="ce462-116">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ce462-117">Relações</span><span class="sxs-lookup"><span data-stu-id="ce462-117">Relationships</span></span>

<span data-ttu-id="ce462-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ce462-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce462-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce462-119">JSON representation</span></span>

<span data-ttu-id="ce462-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce462-120">The following is a JSON representation of the resource.</span></span>

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