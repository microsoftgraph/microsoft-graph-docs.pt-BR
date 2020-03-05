---
title: tipo de recurso labelingOptions
description: Representa as opções de rótulo que podem ser fornecidas para as APIs de avaliação.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 97557ad6e233506e5e074c408ffb04f83297f0af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522999"
---
# <a name="labelingoptions-resource-type"></a><span data-ttu-id="129e7-103">tipo de recurso labelingOptions</span><span class="sxs-lookup"><span data-stu-id="129e7-103">labelingOptions resource type</span></span>

<span data-ttu-id="129e7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="129e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="129e7-105">Representa as opções de rótulo que podem ser fornecidas para as APIs de avaliação.</span><span class="sxs-lookup"><span data-stu-id="129e7-105">Represents the labeling options that can be provided to the evaluation APIs.</span></span> <span data-ttu-id="129e7-106">**labelingOptions** deve ser passado para a API [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) para especificar detalhes sobre o rótulo que deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="129e7-106">**labelingOptions** must be passed in to the [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API to specify details about the label that is to be applied.</span></span> 

## <a name="properties"></a><span data-ttu-id="129e7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="129e7-107">Properties</span></span>

| <span data-ttu-id="129e7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="129e7-108">Property</span></span>               | <span data-ttu-id="129e7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="129e7-109">Type</span></span>                                                | <span data-ttu-id="129e7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="129e7-110">Description</span></span>                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="129e7-111">AssignmentMethod for utilizado</span><span class="sxs-lookup"><span data-stu-id="129e7-111">assignmentMethod</span></span>       | <span data-ttu-id="129e7-112">String</span><span class="sxs-lookup"><span data-stu-id="129e7-112">String</span></span>                                              | <span data-ttu-id="129e7-113">Os valores possíveis são: `standard`, `privileged`, `auto`.</span><span class="sxs-lookup"><span data-stu-id="129e7-113">Possible values are: `standard`, `privileged`, `auto`.</span></span>                                                                        |
| <span data-ttu-id="129e7-114">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="129e7-114">downgradeJustification</span></span> | [<span data-ttu-id="129e7-115">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="129e7-115">downgradeJustification</span></span>](downgradejustification.md) | <span data-ttu-id="129e7-116">O objeto Justification de downgrade que indica se o downgrade foi justificado e, em caso afirmativo, o motivo.</span><span class="sxs-lookup"><span data-stu-id="129e7-116">The downgrade justification object that indicates if downgrade was justified and, if so, the reason.</span></span>                          |
| <span data-ttu-id="129e7-117">extendedProperties</span><span class="sxs-lookup"><span data-stu-id="129e7-117">extendedProperties</span></span>     | <span data-ttu-id="129e7-118">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="129e7-118">[keyValuePair](keyvaluepair.md) collection</span></span>          | <span data-ttu-id="129e7-119">As propriedades estendidas serão analisadas e retornadas no formato de metadados MIP rotulado padrão como parte das informações do rótulo.</span><span class="sxs-lookup"><span data-stu-id="129e7-119">Extended properties will be parsed and returned in the standard MIP labeled metadata format as part of the label information.</span></span> |
| <span data-ttu-id="129e7-120">labelID</span><span class="sxs-lookup"><span data-stu-id="129e7-120">labelId</span></span>                | <span data-ttu-id="129e7-121">Guid</span><span class="sxs-lookup"><span data-stu-id="129e7-121">Guid</span></span>                                                | <span data-ttu-id="129e7-122">O GUID do rótulo que deve ser aplicado à informação.</span><span class="sxs-lookup"><span data-stu-id="129e7-122">The GUID of the label that should be applied to the information.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="129e7-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="129e7-123">JSON representation</span></span>

<span data-ttu-id="129e7-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="129e7-124">The following is a JSON representation of the resource.</span></span>

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