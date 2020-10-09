---
title: tipo de recurso protectDoNotForwardAction
description: Informa ao aplicativo para aplicar a proteção não encaminhar.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8fdb60651e98148eefb7bd964e8c4cd13ff81663
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404382"
---
# <a name="protectdonotforwardaction-resource-type"></a><span data-ttu-id="81836-103">tipo de recurso protectDoNotForwardAction</span><span class="sxs-lookup"><span data-stu-id="81836-103">protectDoNotForwardAction resource type</span></span>

<span data-ttu-id="81836-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81836-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81836-105">Informa ao aplicativo para aplicar a proteção não encaminhar.</span><span class="sxs-lookup"><span data-stu-id="81836-105">Informs the application to apply Do Not Forward protection.</span></span> <span data-ttu-id="81836-106">**protectionDoNotForwardAction** pode ser retornado por [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) ou [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) se o rótulo resultante tiver sido configurado para aplicar a [proteção não encaminhar](/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails).</span><span class="sxs-lookup"><span data-stu-id="81836-106">**protectionDoNotForwardAction** may be returned by [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) or [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) if the resulting label has been configured to apply [Do Not Forward protection](/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails).</span></span> <span data-ttu-id="81836-107">O aplicativo de consumo deve usar uma biblioteca de cliente para aplicar proteção por meio da proteção de informações do Azure.</span><span class="sxs-lookup"><span data-stu-id="81836-107">The consuming application must use a client library to apply protection via Azure Information Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="81836-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81836-108">Properties</span></span>

<span data-ttu-id="81836-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81836-109">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81836-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81836-110">JSON representation</span></span>

<span data-ttu-id="81836-111">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81836-111">The following is a JSON representation of the resource.</span></span>

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