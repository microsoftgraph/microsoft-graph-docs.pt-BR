---
title: tipo de recurso protectByTemplateAction
description: Informa ao aplicativo que um modelo de proteção de proteção de informações do Azure deve ser aplicado.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a7a557dfd72dac9161ae29436f5fc96eb55075d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939071"
---
# <a name="protectbytemplateaction-resource-type"></a><span data-ttu-id="4a8ce-103">tipo de recurso protectByTemplateAction</span><span class="sxs-lookup"><span data-stu-id="4a8ce-103">protectByTemplateAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a8ce-104">Informa ao aplicativo que um modelo de proteção de proteção de informações do Azure deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="4a8ce-104">Informs the application that an Azure Information Protection protection template should be applied.</span></span> <span data-ttu-id="4a8ce-105">**protectionByTemplateAction** pode ser retornado por [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) ou [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) se o rótulo resultante tiver sido configurado para aplicar proteção.</span><span class="sxs-lookup"><span data-stu-id="4a8ce-105">**protectionByTemplateAction** may be returned by [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) or [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) if the resulting label has been configured to apply protection.</span></span> <span data-ttu-id="4a8ce-106">O aplicativo de consumo deve ler o TemplateID do resultado e, em seguida, usar uma biblioteca de cliente, como o SDK do Microsoft Information Protection, para aplicar proteção por meio da proteção de informações do Azure.</span><span class="sxs-lookup"><span data-stu-id="4a8ce-106">The consuming application must read the templateId from the result and then use a client library, such as the Microsoft Information Protection SDK, to apply protection via Azure Information Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="4a8ce-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a8ce-107">Properties</span></span>

| <span data-ttu-id="4a8ce-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a8ce-108">Property</span></span>   | <span data-ttu-id="4a8ce-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a8ce-109">Type</span></span>   | <span data-ttu-id="4a8ce-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a8ce-110">Description</span></span>                                                                        |
| :--------- | :----- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="4a8ce-111">templateId</span><span class="sxs-lookup"><span data-stu-id="4a8ce-111">templateId</span></span> | <span data-ttu-id="4a8ce-112">String</span><span class="sxs-lookup"><span data-stu-id="4a8ce-112">String</span></span> | <span data-ttu-id="4a8ce-113">O GUID do modelo de proteção de informações do Azure a ser aplicado às informações.</span><span class="sxs-lookup"><span data-stu-id="4a8ce-113">The GUID of the Azure Information Protection template to apply to the information.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4a8ce-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a8ce-114">JSON representation</span></span>

<span data-ttu-id="4a8ce-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a8ce-115">The following is a JSON representation of the resource.</span></span>

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