---
title: tipo de recurso protectByTemplateAction
description: Informa ao aplicativo que um modelo de proteção de proteção de informações do Azure deve ser aplicado.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3fc936179a0c0764492a3dc8d677060931a1223a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521366"
---
# <a name="protectbytemplateaction-resource-type"></a><span data-ttu-id="ae6e5-103">tipo de recurso protectByTemplateAction</span><span class="sxs-lookup"><span data-stu-id="ae6e5-103">protectByTemplateAction resource type</span></span>

<span data-ttu-id="ae6e5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ae6e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae6e5-105">Informa ao aplicativo que um modelo de proteção de proteção de informações do Azure deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="ae6e5-105">Informs the application that an Azure Information Protection protection template should be applied.</span></span> <span data-ttu-id="ae6e5-106">**protectionByTemplateAction** pode ser retornado por [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) ou [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) se o rótulo resultante tiver sido configurado para aplicar proteção.</span><span class="sxs-lookup"><span data-stu-id="ae6e5-106">**protectionByTemplateAction** may be returned by [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) or [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) if the resulting label has been configured to apply protection.</span></span> <span data-ttu-id="ae6e5-107">O aplicativo de consumo deve ler o TemplateID do resultado e, em seguida, usar uma biblioteca de cliente, como o SDK do Microsoft Information Protection, para aplicar proteção por meio da proteção de informações do Azure.</span><span class="sxs-lookup"><span data-stu-id="ae6e5-107">The consuming application must read the templateId from the result and then use a client library, such as the Microsoft Information Protection SDK, to apply protection via Azure Information Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="ae6e5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae6e5-108">Properties</span></span>

| <span data-ttu-id="ae6e5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae6e5-109">Property</span></span>   | <span data-ttu-id="ae6e5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae6e5-110">Type</span></span>   | <span data-ttu-id="ae6e5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae6e5-111">Description</span></span>                                                                        |
| :--------- | :----- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="ae6e5-112">templateId</span><span class="sxs-lookup"><span data-stu-id="ae6e5-112">templateId</span></span> | <span data-ttu-id="ae6e5-113">String</span><span class="sxs-lookup"><span data-stu-id="ae6e5-113">String</span></span> | <span data-ttu-id="ae6e5-114">O GUID do modelo de proteção de informações do Azure a ser aplicado às informações.</span><span class="sxs-lookup"><span data-stu-id="ae6e5-114">The GUID of the Azure Information Protection template to apply to the information.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ae6e5-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae6e5-115">JSON representation</span></span>

<span data-ttu-id="ae6e5-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae6e5-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.protectByTemplateAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "templateId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "protectByTemplateAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->