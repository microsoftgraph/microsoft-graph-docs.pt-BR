---
title: tipo de recurso labelingOptions
description: Representa as opções de rótulo que podem ser fornecidas para as APIs de avaliação.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: da2231ae3eb95260663d2907f56f91b96e08278c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084013"
---
# <a name="labelingoptions-resource-type"></a><span data-ttu-id="fe84a-103">tipo de recurso labelingOptions</span><span class="sxs-lookup"><span data-stu-id="fe84a-103">labelingOptions resource type</span></span>

<span data-ttu-id="fe84a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe84a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe84a-105">Representa as opções de rótulo que podem ser fornecidas para as APIs de avaliação.</span><span class="sxs-lookup"><span data-stu-id="fe84a-105">Represents the labeling options that can be provided to the evaluation APIs.</span></span> <span data-ttu-id="fe84a-106">**labelingOptions** deve ser passado para a API [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) para especificar detalhes sobre o rótulo que deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="fe84a-106">**labelingOptions** must be passed in to the [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API to specify details about the label that is to be applied.</span></span> 

## <a name="properties"></a><span data-ttu-id="fe84a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe84a-107">Properties</span></span>

| <span data-ttu-id="fe84a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe84a-108">Property</span></span>               | <span data-ttu-id="fe84a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe84a-109">Type</span></span>                                                | <span data-ttu-id="fe84a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe84a-110">Description</span></span>                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="fe84a-111">AssignmentMethod for utilizado</span><span class="sxs-lookup"><span data-stu-id="fe84a-111">assignmentMethod</span></span>       | <span data-ttu-id="fe84a-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe84a-112">String</span></span>                                              | <span data-ttu-id="fe84a-113">Os valores possíveis são: `standard`, `privileged`, `auto`.</span><span class="sxs-lookup"><span data-stu-id="fe84a-113">Possible values are: `standard`, `privileged`, `auto`.</span></span>                                                                        |
| <span data-ttu-id="fe84a-114">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="fe84a-114">downgradeJustification</span></span> | [<span data-ttu-id="fe84a-115">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="fe84a-115">downgradeJustification</span></span>](downgradejustification.md) | <span data-ttu-id="fe84a-116">O objeto Justification de downgrade que indica se o downgrade foi justificado e, em caso afirmativo, o motivo.</span><span class="sxs-lookup"><span data-stu-id="fe84a-116">The downgrade justification object that indicates if downgrade was justified and, if so, the reason.</span></span>                          |
| <span data-ttu-id="fe84a-117">extendedProperties</span><span class="sxs-lookup"><span data-stu-id="fe84a-117">extendedProperties</span></span>     | <span data-ttu-id="fe84a-118">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="fe84a-118">[keyValuePair](keyvaluepair.md) collection</span></span>          | <span data-ttu-id="fe84a-119">As propriedades estendidas serão analisadas e retornadas no formato de metadados MIP rotulado padrão como parte das informações do rótulo.</span><span class="sxs-lookup"><span data-stu-id="fe84a-119">Extended properties will be parsed and returned in the standard MIP labeled metadata format as part of the label information.</span></span> |
| <span data-ttu-id="fe84a-120">labelID</span><span class="sxs-lookup"><span data-stu-id="fe84a-120">labelId</span></span>                | <span data-ttu-id="fe84a-121">Guid</span><span class="sxs-lookup"><span data-stu-id="fe84a-121">Guid</span></span>                                                | <span data-ttu-id="fe84a-122">O GUID do rótulo que deve ser aplicado à informação.</span><span class="sxs-lookup"><span data-stu-id="fe84a-122">The GUID of the label that should be applied to the information.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="fe84a-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe84a-123">JSON representation</span></span>

<span data-ttu-id="fe84a-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe84a-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.labelingOptions",
  "baseType": null
}-->

```json
{
  "assignmentMethod": "String",
  "downgradeJustification": {"@odata.type": "microsoft.graph.downgradeJustification"},
  "extendedProperties": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "labelId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "labelingOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

