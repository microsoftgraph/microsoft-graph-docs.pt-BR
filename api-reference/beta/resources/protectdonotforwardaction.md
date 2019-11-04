---
title: tipo de recurso protectDoNotForwardAction
description: Informa ao aplicativo para aplicar a proteção não encaminhar.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1d9687460a549438db1c9076bef2184b0b1ee5d3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939184"
---
# <a name="protectdonotforwardaction-resource-type"></a><span data-ttu-id="fd05d-103">tipo de recurso protectDoNotForwardAction</span><span class="sxs-lookup"><span data-stu-id="fd05d-103">protectDoNotForwardAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd05d-104">Informa ao aplicativo para aplicar a proteção não encaminhar.</span><span class="sxs-lookup"><span data-stu-id="fd05d-104">Informs the application to apply Do Not Forward protection.</span></span> <span data-ttu-id="fd05d-105">**protectionDoNotForwardAction** pode ser retornado por [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) ou [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) se o rótulo resultante tiver sido configurado para aplicar a [proteção não encaminhar](https://docs.microsoft.com/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails).</span><span class="sxs-lookup"><span data-stu-id="fd05d-105">**protectionDoNotForwardAction** may be returned by [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) or [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) if the resulting label has been configured to apply [Do Not Forward protection](https://docs.microsoft.com/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails).</span></span> <span data-ttu-id="fd05d-106">O aplicativo de consumo deve usar uma biblioteca de cliente para aplicar proteção por meio da proteção de informações do Azure.</span><span class="sxs-lookup"><span data-stu-id="fd05d-106">The consuming application must use a client library to apply protection via Azure Information Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="fd05d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd05d-107">Properties</span></span>

<span data-ttu-id="fd05d-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fd05d-108">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd05d-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd05d-109">JSON representation</span></span>

<span data-ttu-id="fd05d-110">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fd05d-110">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.protectDoNotForwardAction",
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
  "description": "protectDoNotForwardAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
