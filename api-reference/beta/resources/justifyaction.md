---
title: tipo de recurso justifyaction
description: Indica que uma justificativa é necessária para a operação especificada.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6f2246ad9d166bc51dae79032c95fc3b2d55b72e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523034"
---
# <a name="justifyaction-resource-type"></a><span data-ttu-id="ad40a-103">tipo de recurso justifyaction</span><span class="sxs-lookup"><span data-stu-id="ad40a-103">justifyAction resource type</span></span>

<span data-ttu-id="ad40a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ad40a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad40a-105">Indica que uma justificativa é necessária para a operação especificada.</span><span class="sxs-lookup"><span data-stu-id="ad40a-105">Indicates that a justification is required for the specified operation.</span></span> <span data-ttu-id="ad40a-106">As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) podem retornar **justifyaction**.</span><span class="sxs-lookup"><span data-stu-id="ad40a-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) APIs may return **justifyAction**.</span></span> <span data-ttu-id="ad40a-107">A justificativa é fornecida por meio do [labelingOptions](../resources/labelingoptions.md).</span><span class="sxs-lookup"><span data-stu-id="ad40a-107">Justification is provided via [labelingOptions](../resources/labelingoptions.md).</span></span> <span data-ttu-id="ad40a-108">A chamada anterior deve ser repetida, mas com a propriedade **downgradeJustification** de **labelingOptions** definida com uma mensagem de justificativa, fornecida por meio de entrada do usuário ou lógica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ad40a-108">The previous call should be repeated, but with the **downgradeJustification** property of **labelingOptions** set with a justification message, provided via user input or application logic.</span></span>

## <a name="properties"></a><span data-ttu-id="ad40a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad40a-109">Properties</span></span>

<span data-ttu-id="ad40a-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ad40a-110">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad40a-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad40a-111">JSON representation</span></span>

<span data-ttu-id="ad40a-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ad40a-112">The following is a JSON representation of the resource.</span></span>

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