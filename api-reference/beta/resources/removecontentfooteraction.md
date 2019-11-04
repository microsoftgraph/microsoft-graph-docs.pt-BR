---
title: tipo de recurso removeContentFooterAction
description: Representa uma ação que especifica os detalhes no rodapé de conteúdo a ser removido das informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 62bd0fbefeb9bf246619bc470c5552cd20d174d2
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939443"
---
# <a name="removecontentfooteraction-resource-type"></a><span data-ttu-id="40b9f-103">tipo de recurso removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="40b9f-103">removeContentFooterAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40b9f-104">Representa uma ação que especifica os detalhes no rodapé de conteúdo a ser removido das informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="40b9f-104">Represents an action that specifies the details on the content footer to be removed from the information, if applicable.</span></span> <span data-ttu-id="40b9f-105">As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) podem retornar o **removeContentFooterAction** se o rodapé for removido como resultado da atualização ou remoção do rótulo.</span><span class="sxs-lookup"><span data-stu-id="40b9f-105">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeContentFooterAction** if the footer is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="40b9f-106">A ação instrui o aplicativo de consumo a remover o elemento de interface do usuário específico que contém o rodapé de conteúdo aplicável anteriormente.</span><span class="sxs-lookup"><span data-stu-id="40b9f-106">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content footer.</span></span>

## <a name="properties"></a><span data-ttu-id="40b9f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40b9f-107">Properties</span></span>

| <span data-ttu-id="40b9f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40b9f-108">Property</span></span>       | <span data-ttu-id="40b9f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="40b9f-109">Type</span></span>              | <span data-ttu-id="40b9f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="40b9f-110">Description</span></span>                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| <span data-ttu-id="40b9f-111">uiElementnames</span><span class="sxs-lookup"><span data-stu-id="40b9f-111">uiElementNames</span></span> | <span data-ttu-id="40b9f-112">String collection</span><span class="sxs-lookup"><span data-stu-id="40b9f-112">String collection</span></span> | <span data-ttu-id="40b9f-113">O nome do elemento de interface do usuário do rodapé a ser removido.</span><span class="sxs-lookup"><span data-stu-id="40b9f-113">The name of the UI element of the footer to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="40b9f-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40b9f-114">JSON representation</span></span>

<span data-ttu-id="40b9f-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="40b9f-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeContentFooterAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "uiElementNames": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "removeContentFooterAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->