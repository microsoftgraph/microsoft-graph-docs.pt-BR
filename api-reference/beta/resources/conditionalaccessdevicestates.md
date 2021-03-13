---
title: Tipo de recurso conditionalAccessDeviceStates
description: Representa os estados do dispositivo no escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 152c4edbd641d68f6211111cb29e9794e2a88260
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761797"
---
# <a name="conditionalaccessdevicestates-resource-type"></a><span data-ttu-id="c18b9-103">Tipo de recurso conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="c18b9-103">conditionalAccessDeviceStates resource type</span></span>

<span data-ttu-id="c18b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c18b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c18b9-105">Representa os estados do dispositivo no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="c18b9-105">Represents device states in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="c18b9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c18b9-106">Properties</span></span>

| <span data-ttu-id="c18b9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c18b9-107">Property</span></span>     | <span data-ttu-id="c18b9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c18b9-108">Type</span></span>        | <span data-ttu-id="c18b9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c18b9-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c18b9-110">includeStates</span><span class="sxs-lookup"><span data-stu-id="c18b9-110">includeStates</span></span> | <span data-ttu-id="c18b9-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c18b9-111">String collection</span></span> | <span data-ttu-id="c18b9-112">Estados no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="c18b9-112">States in the scope of the policy.</span></span> <span data-ttu-id="c18b9-113">`All` é o único valor permitido.</span><span class="sxs-lookup"><span data-stu-id="c18b9-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="c18b9-114">excludeStates</span><span class="sxs-lookup"><span data-stu-id="c18b9-114">excludeStates</span></span> | <span data-ttu-id="c18b9-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c18b9-115">String collection</span></span> | <span data-ttu-id="c18b9-116">Estados excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="c18b9-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="c18b9-117">Valores possíveis: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="c18b9-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c18b9-118">Relações</span><span class="sxs-lookup"><span data-stu-id="c18b9-118">Relationships</span></span>

<span data-ttu-id="c18b9-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c18b9-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c18b9-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c18b9-120">JSON representation</span></span>

<span data-ttu-id="c18b9-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c18b9-121">The following is a JSON representation of the resource.</span></span>

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

