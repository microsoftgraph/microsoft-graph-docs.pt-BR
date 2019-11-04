---
title: tipo de recurso applyLabelAction
description: Representa um conjunto de ações que devem ser seguidas para aplicar ou atualizar um rótulo.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fc7911b3a225f226edc74dc9b194a2522b7c4251
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939142"
---
# <a name="applylabelaction-resource-type"></a><span data-ttu-id="82f31-103">tipo de recurso applyLabelAction</span><span class="sxs-lookup"><span data-stu-id="82f31-103">applyLabelAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82f31-104">Representa um conjunto de ações que devem ser seguidas para aplicar ou atualizar um rótulo.</span><span class="sxs-lookup"><span data-stu-id="82f31-104">Represents a set of actions that should be taken to apply or update a label.</span></span> <span data-ttu-id="82f31-105">**applyLabelAction** é retornado quando o resultado de uma operação de avaliação de rótulo é que um rótulo deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="82f31-105">**applyLabelAction** is returned when the result of a label evaluation operation is that a label should be applied.</span></span> <span data-ttu-id="82f31-106">A `actions` propriedade contém uma coleção [informationProtectionAction](informationProtectionaction.md) que descreveu o conjunto completo de ações para *aplicar* o rótulo, incluindo remoção de metadados antigos, marcação de conteúdo e proteção.</span><span class="sxs-lookup"><span data-stu-id="82f31-106">The `actions` property contains an [informationProtectionAction](informationProtectionaction.md) collection that described the full set of actions to *apply* the label, including removal of old metadata, content marking, and protection.</span></span>

## <a name="properties"></a><span data-ttu-id="82f31-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82f31-107">Properties</span></span>

| <span data-ttu-id="82f31-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82f31-108">Property</span></span>                    | <span data-ttu-id="82f31-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="82f31-109">Type</span></span>                                                                     | <span data-ttu-id="82f31-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="82f31-110">Description</span></span>                                                                                                                                                                                       |
| :-------------------------- | :----------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="82f31-111">ação</span><span class="sxs-lookup"><span data-stu-id="82f31-111">actionSource</span></span>                | <span data-ttu-id="82f31-112">String</span><span class="sxs-lookup"><span data-stu-id="82f31-112">String</span></span>                                                                   | <span data-ttu-id="82f31-113">Os valores possíveis são: `manual`, `automatic`, `recommended`, `default`.</span><span class="sxs-lookup"><span data-stu-id="82f31-113">Possible values are: `manual`, `automatic`, `recommended`, `default`.</span></span>                                                                                                                             |
| <span data-ttu-id="82f31-114">actions</span><span class="sxs-lookup"><span data-stu-id="82f31-114">actions</span></span>                     | <span data-ttu-id="82f31-115">coleção [informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="82f31-115">[informationProtectionAction](informationprotectionaction.md) collection</span></span> | <span data-ttu-id="82f31-116">A coleção de ações específicas que devem ser tomadas pelo aplicativo de consumo para rotular o documento.</span><span class="sxs-lookup"><span data-stu-id="82f31-116">The collection of specific actions that should be taken by the consuming application to label the document.</span></span> <span data-ttu-id="82f31-117">Consulte [informationProtectionAction](informationprotectionaction.md) para obter a lista completa.</span><span class="sxs-lookup"><span data-stu-id="82f31-117">See  [informationProtectionAction](informationprotectionaction.md) for the full list.</span></span> |
| <span data-ttu-id="82f31-118">rótulo</span><span class="sxs-lookup"><span data-stu-id="82f31-118">label</span></span>                       | [<span data-ttu-id="82f31-119">labelDetails</span><span class="sxs-lookup"><span data-stu-id="82f31-119">labelDetails</span></span>](labeldetails.md)                                          | <span data-ttu-id="82f31-120">Objeto que descreve os detalhes do rótulo a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="82f31-120">Object that describes the details of the label to apply.</span></span>                                                                                                                                          |
| <span data-ttu-id="82f31-121">responsibleSensitiveTypeIds</span><span class="sxs-lookup"><span data-stu-id="82f31-121">responsibleSensitiveTypeIds</span></span> | <span data-ttu-id="82f31-122">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="82f31-122">Guid collection</span></span>                                                          | <span data-ttu-id="82f31-123">Se o rótulo foi o resultado de uma classificação automática, forneça a lista de GUIDs de tipo de informações confidenciais que resultaram no rótulo retornado.</span><span class="sxs-lookup"><span data-stu-id="82f31-123">If the label was the result of an automatic classification, supply the list of sensitive info type GUIDs that resulted in the returned label.</span></span>                                         
## <a name="json-representation"></a><span data-ttu-id="82f31-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82f31-124">JSON representation</span></span>

<span data-ttu-id="82f31-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="82f31-125">The following is a JSON representation of the resource.</span></span>

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