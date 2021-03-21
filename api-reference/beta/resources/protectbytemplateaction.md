---
title: Tipo de recurso protectByTemplateAction
description: Informa ao aplicativo que um modelo de proteção de informações do Azure deve ser aplicado.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6524774af3faa496b141e37ec270f8a73770ee63
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956824"
---
# <a name="protectbytemplateaction-resource-type"></a><span data-ttu-id="9cf40-103">Tipo de recurso protectByTemplateAction</span><span class="sxs-lookup"><span data-stu-id="9cf40-103">protectByTemplateAction resource type</span></span>

<span data-ttu-id="9cf40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cf40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cf40-105">Informa ao aplicativo que um modelo de proteção de informações do Azure deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="9cf40-105">Informs the application that an Azure Information Protection protection template should be applied.</span></span> <span data-ttu-id="9cf40-106">**protectionByTemplateAction** pode ser retornado por [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) ou [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) se o rótulo resultante tiver sido configurado para aplicar proteção.</span><span class="sxs-lookup"><span data-stu-id="9cf40-106">**protectionByTemplateAction** may be returned by [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) or [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) if the resulting label has been configured to apply protection.</span></span> <span data-ttu-id="9cf40-107">O aplicativo de consumo deve ler o templateId do resultado e, em seguida, usar uma biblioteca de clientes, como o SDK da Proteção de Informações da Microsoft, para aplicar proteção por meio da Proteção de Informações do Azure.</span><span class="sxs-lookup"><span data-stu-id="9cf40-107">The consuming application must read the templateId from the result and then use a client library, such as the Microsoft Information Protection SDK, to apply protection via Azure Information Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="9cf40-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9cf40-108">Properties</span></span>

| <span data-ttu-id="9cf40-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9cf40-109">Property</span></span>   | <span data-ttu-id="9cf40-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cf40-110">Type</span></span>   | <span data-ttu-id="9cf40-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cf40-111">Description</span></span>                                                                        |
| :--------- | :----- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="9cf40-112">templateId</span><span class="sxs-lookup"><span data-stu-id="9cf40-112">templateId</span></span> | <span data-ttu-id="9cf40-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cf40-113">String</span></span> | <span data-ttu-id="9cf40-114">O GUID do modelo de Proteção de Informações do Azure a ser aplicado às informações.</span><span class="sxs-lookup"><span data-stu-id="9cf40-114">The GUID of the Azure Information Protection template to apply to the information.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9cf40-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9cf40-115">JSON representation</span></span>

<span data-ttu-id="9cf40-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9cf40-116">The following is a JSON representation of the resource.</span></span>

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

