---
title: tipo de recurso removeWatermarkAction
description: Representa uma ação que especifica os detalhes sobre a marca d' água de conteúdo a ser removido das informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 34859dedd5e5e740aa776cdf78bb742399523fa2
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939268"
---
# <a name="removewatermarkaction-resource-type"></a><span data-ttu-id="714f7-103">tipo de recurso removeWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="714f7-103">removeWatermarkAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="714f7-104">Representa uma ação que especifica os detalhes sobre a marca d' água de conteúdo a ser removido das informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="714f7-104">Represents an action that specifies the details on the content watermark to be removed from the information, if applicable.</span></span> <span data-ttu-id="714f7-105">As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) podem retornar o **removeWatermarkAction** se a marca d' água for removida como resultado da atualização ou remoção do rótulo.</span><span class="sxs-lookup"><span data-stu-id="714f7-105">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeWatermarkAction** if the watermark is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="714f7-106">A ação instrui o aplicativo de consumo a remover o elemento de interface do usuário específico que contém a marca d' água de conteúdo aplicável anteriormente.</span><span class="sxs-lookup"><span data-stu-id="714f7-106">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content watermark.</span></span>

## <a name="properties"></a><span data-ttu-id="714f7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="714f7-107">Properties</span></span>

| <span data-ttu-id="714f7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="714f7-108">Property</span></span>       | <span data-ttu-id="714f7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="714f7-109">Type</span></span>              | <span data-ttu-id="714f7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="714f7-110">Description</span></span>                           |
| :------------- | :---------------- | :------------------------------------ |
| <span data-ttu-id="714f7-111">uiElementnames</span><span class="sxs-lookup"><span data-stu-id="714f7-111">uiElementNames</span></span> | <span data-ttu-id="714f7-112">String collection</span><span class="sxs-lookup"><span data-stu-id="714f7-112">String collection</span></span> | <span data-ttu-id="714f7-113">O nome do elemento de interface do usuário do rodapé a ser removido.</span><span class="sxs-lookup"><span data-stu-id="714f7-113">The name of the UI element of footer to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="714f7-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="714f7-114">JSON representation</span></span>

<span data-ttu-id="714f7-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="714f7-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeWatermarkAction",
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
  "description": "removeWatermarkAction resource",
  "keywords": "",  
  "section": "documentation",
  "tocPath": ""
}-->