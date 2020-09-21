---
title: tipo de recurso applyLabelAction
description: Representa um conjunto de ações que devem ser seguidas para aplicar ou atualizar um rótulo.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2ea3d99ddd22056f9a3413f047a20387bf22a934
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050224"
---
# <a name="applylabelaction-resource-type"></a><span data-ttu-id="32c7d-103">tipo de recurso applyLabelAction</span><span class="sxs-lookup"><span data-stu-id="32c7d-103">applyLabelAction resource type</span></span>

<span data-ttu-id="32c7d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32c7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32c7d-105">Representa um conjunto de ações que devem ser seguidas para aplicar ou atualizar um rótulo.</span><span class="sxs-lookup"><span data-stu-id="32c7d-105">Represents a set of actions that should be taken to apply or update a label.</span></span> <span data-ttu-id="32c7d-106">**applyLabelAction** é retornado quando o resultado de uma operação de avaliação de rótulo é que um rótulo deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="32c7d-106">**applyLabelAction** is returned when the result of a label evaluation operation is that a label should be applied.</span></span> <span data-ttu-id="32c7d-107">A `actions` propriedade contém uma coleção [informationProtectionAction](informationProtectionaction.md) que descreveu o conjunto completo de ações para *aplicar* o rótulo, incluindo remoção de metadados antigos, marcação de conteúdo e proteção.</span><span class="sxs-lookup"><span data-stu-id="32c7d-107">The `actions` property contains an [informationProtectionAction](informationProtectionaction.md) collection that described the full set of actions to *apply* the label, including removal of old metadata, content marking, and protection.</span></span>

## <a name="properties"></a><span data-ttu-id="32c7d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32c7d-108">Properties</span></span>

| <span data-ttu-id="32c7d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32c7d-109">Property</span></span>                    | <span data-ttu-id="32c7d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="32c7d-110">Type</span></span>                                                                     | <span data-ttu-id="32c7d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="32c7d-111">Description</span></span>                                                                                                                                                                                       |
| :-------------------------- | :----------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="32c7d-112">ação</span><span class="sxs-lookup"><span data-stu-id="32c7d-112">actionSource</span></span>                | <span data-ttu-id="32c7d-113">String</span><span class="sxs-lookup"><span data-stu-id="32c7d-113">String</span></span>                                                                   | <span data-ttu-id="32c7d-114">Os valores possíveis são: `manual`, `automatic`, `recommended`, `default`.</span><span class="sxs-lookup"><span data-stu-id="32c7d-114">Possible values are: `manual`, `automatic`, `recommended`, `default`.</span></span>                                                                                                                             |
| <span data-ttu-id="32c7d-115">actions</span><span class="sxs-lookup"><span data-stu-id="32c7d-115">actions</span></span>                     | <span data-ttu-id="32c7d-116">coleção [informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="32c7d-116">[informationProtectionAction](informationprotectionaction.md) collection</span></span> | <span data-ttu-id="32c7d-117">A coleção de ações específicas que devem ser tomadas pelo aplicativo de consumo para rotular o documento.</span><span class="sxs-lookup"><span data-stu-id="32c7d-117">The collection of specific actions that should be taken by the consuming application to label the document.</span></span> <span data-ttu-id="32c7d-118">Consulte  [informationProtectionAction](informationprotectionaction.md) para obter a lista completa.</span><span class="sxs-lookup"><span data-stu-id="32c7d-118">See  [informationProtectionAction](informationprotectionaction.md) for the full list.</span></span> |
| <span data-ttu-id="32c7d-119">rótulo</span><span class="sxs-lookup"><span data-stu-id="32c7d-119">label</span></span>                       | [<span data-ttu-id="32c7d-120">labelDetails</span><span class="sxs-lookup"><span data-stu-id="32c7d-120">labelDetails</span></span>](labeldetails.md)                                          | <span data-ttu-id="32c7d-121">Objeto que descreve os detalhes do rótulo a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="32c7d-121">Object that describes the details of the label to apply.</span></span>                                                                                                                                          |
| <span data-ttu-id="32c7d-122">responsibleSensitiveTypeIds</span><span class="sxs-lookup"><span data-stu-id="32c7d-122">responsibleSensitiveTypeIds</span></span> | <span data-ttu-id="32c7d-123">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="32c7d-123">Guid collection</span></span>                                                          | <span data-ttu-id="32c7d-124">Se o rótulo foi o resultado de uma classificação automática, forneça a lista de GUIDs de tipo de informações confidenciais que resultaram no rótulo retornado.</span><span class="sxs-lookup"><span data-stu-id="32c7d-124">If the label was the result of an automatic classification, supply the list of sensitive info type GUIDs that resulted in the returned label.</span></span>                                         
## <a name="json-representation"></a><span data-ttu-id="32c7d-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32c7d-125">JSON representation</span></span>

<span data-ttu-id="32c7d-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32c7d-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applyLabelAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "actionSource": "String",
  "actions": [{"@odata.type": "microsoft.graph.informationProtectionAction"}],
  "label": {"@odata.type": "microsoft.graph.labelDetails"},
  "responsibleSensitiveTypeIds": ["Guid"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applyLabelAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

