---
title: tipo de recurso justifyaction
description: Indica que uma justificativa é necessária para a operação especificada.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9e26cd675ecb1a3a50c505c019244c60eaee88c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039353"
---
# <a name="justifyaction-resource-type"></a><span data-ttu-id="884ea-103">tipo de recurso justifyaction</span><span class="sxs-lookup"><span data-stu-id="884ea-103">justifyAction resource type</span></span>

<span data-ttu-id="884ea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="884ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="884ea-105">Indica que uma justificativa é necessária para a operação especificada.</span><span class="sxs-lookup"><span data-stu-id="884ea-105">Indicates that a justification is required for the specified operation.</span></span> <span data-ttu-id="884ea-106">As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) podem retornar **justifyaction**.</span><span class="sxs-lookup"><span data-stu-id="884ea-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) APIs may return **justifyAction**.</span></span> <span data-ttu-id="884ea-107">A justificativa é fornecida por meio do [labelingOptions](../resources/labelingoptions.md).</span><span class="sxs-lookup"><span data-stu-id="884ea-107">Justification is provided via [labelingOptions](../resources/labelingoptions.md).</span></span> <span data-ttu-id="884ea-108">A chamada anterior deve ser repetida, mas com a propriedade **downgradeJustification** de **labelingOptions** definida com uma mensagem de justificativa, fornecida por meio de entrada do usuário ou lógica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="884ea-108">The previous call should be repeated, but with the **downgradeJustification** property of **labelingOptions** set with a justification message, provided via user input or application logic.</span></span>

## <a name="properties"></a><span data-ttu-id="884ea-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="884ea-109">Properties</span></span>

<span data-ttu-id="884ea-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="884ea-110">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="884ea-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="884ea-111">JSON representation</span></span>

<span data-ttu-id="884ea-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="884ea-112">The following is a JSON representation of the resource.</span></span>

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

