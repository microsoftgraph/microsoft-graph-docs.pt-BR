---
title: tipo de recurso labelingOptions
description: Representa as opções de rótulo que podem ser fornecidas para as APIs de avaliação.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f8883c08bbd1f351dc5de003988f36c727ef85d7
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939296"
---
# <a name="labelingoptions-resource-type"></a><span data-ttu-id="f3778-103">tipo de recurso labelingOptions</span><span class="sxs-lookup"><span data-stu-id="f3778-103">labelingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3778-104">Representa as opções de rótulo que podem ser fornecidas para as APIs de avaliação.</span><span class="sxs-lookup"><span data-stu-id="f3778-104">Represents the labeling options that can be provided to the evaluation APIs.</span></span> <span data-ttu-id="f3778-105">**labelingOptions** deve ser passado para a API [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) para especificar detalhes sobre o rótulo que deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="f3778-105">**labelingOptions** must be passed in to the [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API to specify details about the label that is to be applied.</span></span> 

## <a name="properties"></a><span data-ttu-id="f3778-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3778-106">Properties</span></span>

| <span data-ttu-id="f3778-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3778-107">Property</span></span>               | <span data-ttu-id="f3778-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3778-108">Type</span></span>                                                | <span data-ttu-id="f3778-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3778-109">Description</span></span>                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f3778-110">AssignmentMethod for utilizado</span><span class="sxs-lookup"><span data-stu-id="f3778-110">assignmentMethod</span></span>       | <span data-ttu-id="f3778-111">String</span><span class="sxs-lookup"><span data-stu-id="f3778-111">String</span></span>                                              | <span data-ttu-id="f3778-112">Os valores possíveis são: `standard`, `privileged`, `auto`.</span><span class="sxs-lookup"><span data-stu-id="f3778-112">Possible values are: `standard`, `privileged`, `auto`.</span></span>                                                                        |
| <span data-ttu-id="f3778-113">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="f3778-113">downgradeJustification</span></span> | [<span data-ttu-id="f3778-114">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="f3778-114">downgradeJustification</span></span>](downgradejustification.md) | <span data-ttu-id="f3778-115">O objeto Justification de downgrade que indica se o downgrade foi justificado e, em caso afirmativo, o motivo.</span><span class="sxs-lookup"><span data-stu-id="f3778-115">The downgrade justification object that indicates if downgrade was justified and, if so, the reason.</span></span>                          |
| <span data-ttu-id="f3778-116">extendedProperties</span><span class="sxs-lookup"><span data-stu-id="f3778-116">extendedProperties</span></span>     | <span data-ttu-id="f3778-117">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f3778-117">[keyValuePair](keyvaluepair.md) collection</span></span>          | <span data-ttu-id="f3778-118">As propriedades estendidas serão analisadas e retornadas no formato de metadados MIP rotulado padrão como parte das informações do rótulo.</span><span class="sxs-lookup"><span data-stu-id="f3778-118">Extended properties will be parsed and returned in the standard MIP labeled metadata format as part of the label information.</span></span> |
| <span data-ttu-id="f3778-119">labelID</span><span class="sxs-lookup"><span data-stu-id="f3778-119">labelId</span></span>                | <span data-ttu-id="f3778-120">Guid</span><span class="sxs-lookup"><span data-stu-id="f3778-120">Guid</span></span>                                                | <span data-ttu-id="f3778-121">O GUID do rótulo que deve ser aplicado à informação.</span><span class="sxs-lookup"><span data-stu-id="f3778-121">The GUID of the label that should be applied to the information.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="f3778-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3778-122">JSON representation</span></span>

<span data-ttu-id="f3778-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3778-123">The following is a JSON representation of the resource.</span></span>

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