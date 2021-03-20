---
title: Tipo de recurso protectDoNotForwardAction
description: Informa ao aplicativo para aplicar a proteção Não Encaminhar.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: a68771ea278ba8a904c032a86732b2b190eeeb43
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941768"
---
# <a name="protectdonotforwardaction-resource-type"></a><span data-ttu-id="58986-103">Tipo de recurso protectDoNotForwardAction</span><span class="sxs-lookup"><span data-stu-id="58986-103">protectDoNotForwardAction resource type</span></span>

<span data-ttu-id="58986-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58986-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58986-105">Informa ao aplicativo para aplicar a proteção Não Encaminhar.</span><span class="sxs-lookup"><span data-stu-id="58986-105">Informs the application to apply Do Not Forward protection.</span></span> <span data-ttu-id="58986-106">**protectionDoNotForwardAction** poderá ser retornado por [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) ou [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) se o rótulo resultante tiver sido configurado para aplicar a proteção [Não Encaminhar](/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails).</span><span class="sxs-lookup"><span data-stu-id="58986-106">**protectionDoNotForwardAction** may be returned by [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) or [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) if the resulting label has been configured to apply [Do Not Forward protection](/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails).</span></span> <span data-ttu-id="58986-107">O aplicativo de consumo deve usar uma biblioteca de clientes para aplicar proteção por meio da Proteção de Informações do Azure.</span><span class="sxs-lookup"><span data-stu-id="58986-107">The consuming application must use a client library to apply protection via Azure Information Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="58986-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58986-108">Properties</span></span>

<span data-ttu-id="58986-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58986-109">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58986-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58986-110">JSON representation</span></span>

<span data-ttu-id="58986-111">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="58986-111">The following is a JSON representation of the resource.</span></span>

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