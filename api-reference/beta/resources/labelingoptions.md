---
title: Tipo de recurso labelingOptions
description: Representa as opções de rotulagem que podem ser fornecidas às APIs de avaliação.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7d2409bf538de3d37ca32cdf2fd1afb78a659817
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950295"
---
# <a name="labelingoptions-resource-type"></a><span data-ttu-id="51b21-103">Tipo de recurso labelingOptions</span><span class="sxs-lookup"><span data-stu-id="51b21-103">labelingOptions resource type</span></span>

<span data-ttu-id="51b21-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51b21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51b21-105">Representa as opções de rotulagem que podem ser fornecidas às APIs de avaliação.</span><span class="sxs-lookup"><span data-stu-id="51b21-105">Represents the labeling options that can be provided to the evaluation APIs.</span></span> <span data-ttu-id="51b21-106">**labelingOptions** deve ser passado para a API [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) para especificar detalhes sobre o rótulo a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="51b21-106">**labelingOptions** must be passed in to the [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API to specify details about the label that is to be applied.</span></span> 

## <a name="properties"></a><span data-ttu-id="51b21-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51b21-107">Properties</span></span>

| <span data-ttu-id="51b21-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51b21-108">Property</span></span>               | <span data-ttu-id="51b21-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="51b21-109">Type</span></span>                                                | <span data-ttu-id="51b21-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="51b21-110">Description</span></span>                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="51b21-111">assignmentMethod</span><span class="sxs-lookup"><span data-stu-id="51b21-111">assignmentMethod</span></span>       | <span data-ttu-id="51b21-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51b21-112">String</span></span>                                              | <span data-ttu-id="51b21-113">Os valores possíveis são: `standard`, `privileged`, `auto`.</span><span class="sxs-lookup"><span data-stu-id="51b21-113">Possible values are: `standard`, `privileged`, `auto`.</span></span>                                                                        |
| <span data-ttu-id="51b21-114">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="51b21-114">downgradeJustification</span></span> | [<span data-ttu-id="51b21-115">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="51b21-115">downgradeJustification</span></span>](downgradejustification.md) | <span data-ttu-id="51b21-116">O objeto de justificativa de downgrade que indica se downgrade foi justificado e, em caso afirmado, o motivo.</span><span class="sxs-lookup"><span data-stu-id="51b21-116">The downgrade justification object that indicates if downgrade was justified and, if so, the reason.</span></span>                          |
| <span data-ttu-id="51b21-117">extendedProperties</span><span class="sxs-lookup"><span data-stu-id="51b21-117">extendedProperties</span></span>     | <span data-ttu-id="51b21-118">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="51b21-118">[keyValuePair](keyvaluepair.md) collection</span></span>          | <span data-ttu-id="51b21-119">As propriedades estendidas serão analisados e retornadas no formato de metadados padrão rotulados MIP como parte das informações do rótulo.</span><span class="sxs-lookup"><span data-stu-id="51b21-119">Extended properties will be parsed and returned in the standard MIP labeled metadata format as part of the label information.</span></span> |
| <span data-ttu-id="51b21-120">labelId</span><span class="sxs-lookup"><span data-stu-id="51b21-120">labelId</span></span>                | <span data-ttu-id="51b21-121">Guid</span><span class="sxs-lookup"><span data-stu-id="51b21-121">Guid</span></span>                                                | <span data-ttu-id="51b21-122">O GUID do rótulo que deve ser aplicado às informações.</span><span class="sxs-lookup"><span data-stu-id="51b21-122">The GUID of the label that should be applied to the information.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="51b21-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51b21-123">JSON representation</span></span>

<span data-ttu-id="51b21-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51b21-124">The following is a JSON representation of the resource.</span></span>

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

