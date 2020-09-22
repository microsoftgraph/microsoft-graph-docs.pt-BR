---
title: tipo de recurso removeContentFooterAction
description: Representa uma ação que especifica os detalhes no rodapé de conteúdo a ser removido das informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 76450b0d6b0f3a532a4e3472d2ce99ead8c933e4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073443"
---
# <a name="removecontentfooteraction-resource-type"></a><span data-ttu-id="f1dd9-103">tipo de recurso removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="f1dd9-103">removeContentFooterAction resource type</span></span>

<span data-ttu-id="f1dd9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1dd9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1dd9-105">Representa uma ação que especifica os detalhes no rodapé de conteúdo a ser removido das informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="f1dd9-105">Represents an action that specifies the details on the content footer to be removed from the information, if applicable.</span></span> <span data-ttu-id="f1dd9-106">As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) podem retornar o **removeContentFooterAction** se o rodapé for removido como resultado da atualização ou remoção do rótulo.</span><span class="sxs-lookup"><span data-stu-id="f1dd9-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeContentFooterAction** if the footer is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="f1dd9-107">A ação instrui o aplicativo de consumo a remover o elemento de interface do usuário específico que contém o rodapé de conteúdo aplicável anteriormente.</span><span class="sxs-lookup"><span data-stu-id="f1dd9-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content footer.</span></span>

## <a name="properties"></a><span data-ttu-id="f1dd9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1dd9-108">Properties</span></span>

| <span data-ttu-id="f1dd9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1dd9-109">Property</span></span>       | <span data-ttu-id="f1dd9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1dd9-110">Type</span></span>              | <span data-ttu-id="f1dd9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1dd9-111">Description</span></span>                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| <span data-ttu-id="f1dd9-112">uiElementnames</span><span class="sxs-lookup"><span data-stu-id="f1dd9-112">uiElementNames</span></span> | <span data-ttu-id="f1dd9-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1dd9-113">String collection</span></span> | <span data-ttu-id="f1dd9-114">O nome do elemento de interface do usuário do rodapé a ser removido.</span><span class="sxs-lookup"><span data-stu-id="f1dd9-114">The name of the UI element of the footer to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f1dd9-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1dd9-115">JSON representation</span></span>

<span data-ttu-id="f1dd9-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1dd9-116">The following is a JSON representation of the resource.</span></span>

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

