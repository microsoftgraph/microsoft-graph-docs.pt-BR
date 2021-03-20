---
title: Tipo de recurso applyLabelAction
description: Representa um conjunto de ações que devem ser tomadas para aplicar ou atualizar um rótulo.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e53a2796c7cd4f0b8c0a415ca4bc38ffefeb609e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945736"
---
# <a name="applylabelaction-resource-type"></a><span data-ttu-id="89a16-103">Tipo de recurso applyLabelAction</span><span class="sxs-lookup"><span data-stu-id="89a16-103">applyLabelAction resource type</span></span>

<span data-ttu-id="89a16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89a16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89a16-105">Representa um conjunto de ações que devem ser tomadas para aplicar ou atualizar um rótulo.</span><span class="sxs-lookup"><span data-stu-id="89a16-105">Represents a set of actions that should be taken to apply or update a label.</span></span> <span data-ttu-id="89a16-106">**applyLabelAction** é retornado quando o resultado de uma operação de avaliação de rótulo é que um rótulo deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="89a16-106">**applyLabelAction** is returned when the result of a label evaluation operation is that a label should be applied.</span></span> <span data-ttu-id="89a16-107">A `actions` propriedade contém uma coleção [informationProtectionAction](informationProtectionaction.md) que  descreve o conjunto completo de ações para aplicar o rótulo, incluindo a remoção de metadados antigos, marcação de conteúdo e proteção.</span><span class="sxs-lookup"><span data-stu-id="89a16-107">The `actions` property contains an [informationProtectionAction](informationProtectionaction.md) collection that described the full set of actions to *apply* the label, including removal of old metadata, content marking, and protection.</span></span>

## <a name="properties"></a><span data-ttu-id="89a16-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89a16-108">Properties</span></span>

| <span data-ttu-id="89a16-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89a16-109">Property</span></span>                    | <span data-ttu-id="89a16-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="89a16-110">Type</span></span>                                                                     | <span data-ttu-id="89a16-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="89a16-111">Description</span></span>                                                                                                                                                                                       |
| :-------------------------- | :----------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="89a16-112">actionSource</span><span class="sxs-lookup"><span data-stu-id="89a16-112">actionSource</span></span>                | <span data-ttu-id="89a16-113">String</span><span class="sxs-lookup"><span data-stu-id="89a16-113">String</span></span>                                                                   | <span data-ttu-id="89a16-114">Os valores possíveis são: `manual`, `automatic`, `recommended`, `default`.</span><span class="sxs-lookup"><span data-stu-id="89a16-114">Possible values are: `manual`, `automatic`, `recommended`, `default`.</span></span>                                                                                                                             |
| <span data-ttu-id="89a16-115">actions</span><span class="sxs-lookup"><span data-stu-id="89a16-115">actions</span></span>                     | <span data-ttu-id="89a16-116">[Coleção informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="89a16-116">[informationProtectionAction](informationprotectionaction.md) collection</span></span> | <span data-ttu-id="89a16-117">O conjunto de ações específicas que devem ser tomadas pelo aplicativo de consumo para rotular o documento.</span><span class="sxs-lookup"><span data-stu-id="89a16-117">The collection of specific actions that should be taken by the consuming application to label the document.</span></span> <span data-ttu-id="89a16-118">Consulte  [informationProtectionAction](informationprotectionaction.md) para obter a lista completa.</span><span class="sxs-lookup"><span data-stu-id="89a16-118">See  [informationProtectionAction](informationprotectionaction.md) for the full list.</span></span> |
| <span data-ttu-id="89a16-119">rótulo</span><span class="sxs-lookup"><span data-stu-id="89a16-119">label</span></span>                       | [<span data-ttu-id="89a16-120">labelDetails</span><span class="sxs-lookup"><span data-stu-id="89a16-120">labelDetails</span></span>](labeldetails.md)                                          | <span data-ttu-id="89a16-121">Objeto que descreve os detalhes do rótulo a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="89a16-121">Object that describes the details of the label to apply.</span></span>                                                                                                                                          |
| <span data-ttu-id="89a16-122">responsibleSensitiveTypeIds</span><span class="sxs-lookup"><span data-stu-id="89a16-122">responsibleSensitiveTypeIds</span></span> | <span data-ttu-id="89a16-123">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="89a16-123">Guid collection</span></span>                                                          | <span data-ttu-id="89a16-124">Se o rótulo foi o resultado de uma classificação automática, fornece a lista de GUIDs do tipo de informação confidenciais que resultaram no rótulo retornado.</span><span class="sxs-lookup"><span data-stu-id="89a16-124">If the label was the result of an automatic classification, supply the list of sensitive info type GUIDs that resulted in the returned label.</span></span>                                         
## <a name="json-representation"></a><span data-ttu-id="89a16-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89a16-125">JSON representation</span></span>

<span data-ttu-id="89a16-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89a16-126">The following is a JSON representation of the resource.</span></span>

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

