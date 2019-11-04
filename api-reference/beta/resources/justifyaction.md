---
title: tipo de recurso justifyaction
description: Indica que uma justificativa é necessária para a operação especificada.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bc96062febc15310de6a3b2ed04f96a8cf1e69e5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939310"
---
# <a name="justifyaction-resource-type"></a><span data-ttu-id="c5c9a-103">tipo de recurso justifyaction</span><span class="sxs-lookup"><span data-stu-id="c5c9a-103">justifyAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5c9a-104">Indica que uma justificativa é necessária para a operação especificada.</span><span class="sxs-lookup"><span data-stu-id="c5c9a-104">Indicates that a justification is required for the specified operation.</span></span> <span data-ttu-id="c5c9a-105">As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) podem retornar **justifyaction**.</span><span class="sxs-lookup"><span data-stu-id="c5c9a-105">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) APIs may return **justifyAction**.</span></span> <span data-ttu-id="c5c9a-106">A justificativa é fornecida por meio do [labelingOptions](../resources/labelingoptions.md).</span><span class="sxs-lookup"><span data-stu-id="c5c9a-106">Justification is provided via [labelingOptions](../resources/labelingoptions.md).</span></span> <span data-ttu-id="c5c9a-107">A chamada anterior deve ser repetida, mas com a propriedade **downgradeJustification** de **labelingOptions** definida com uma mensagem de justificativa, fornecida por meio de entrada do usuário ou lógica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c5c9a-107">The previous call should be repeated, but with the **downgradeJustification** property of **labelingOptions** set with a justification message, provided via user input or application logic.</span></span>

## <a name="properties"></a><span data-ttu-id="c5c9a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5c9a-108">Properties</span></span>

<span data-ttu-id="c5c9a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c5c9a-109">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5c9a-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5c9a-110">JSON representation</span></span>

<span data-ttu-id="c5c9a-111">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5c9a-111">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.justifyAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "justifyAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->