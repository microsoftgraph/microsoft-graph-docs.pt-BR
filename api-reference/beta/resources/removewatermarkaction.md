---
title: tipo de recurso removeWatermarkAction
description: Representa uma ação que especifica os detalhes sobre a marca d' água de conteúdo a ser removido das informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 271058e3ae56b2ded72c577f453d2af920d3ef0c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521135"
---
# <a name="removewatermarkaction-resource-type"></a><span data-ttu-id="1f606-103">tipo de recurso removeWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="1f606-103">removeWatermarkAction resource type</span></span>

<span data-ttu-id="1f606-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1f606-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f606-105">Representa uma ação que especifica os detalhes sobre a marca d' água de conteúdo a ser removido das informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="1f606-105">Represents an action that specifies the details on the content watermark to be removed from the information, if applicable.</span></span> <span data-ttu-id="1f606-106">As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) podem retornar o **removeWatermarkAction** se a marca d' água for removida como resultado da atualização ou remoção do rótulo.</span><span class="sxs-lookup"><span data-stu-id="1f606-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeWatermarkAction** if the watermark is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="1f606-107">A ação instrui o aplicativo de consumo a remover o elemento de interface do usuário específico que contém a marca d' água de conteúdo aplicável anteriormente.</span><span class="sxs-lookup"><span data-stu-id="1f606-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content watermark.</span></span>

## <a name="properties"></a><span data-ttu-id="1f606-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f606-108">Properties</span></span>

| <span data-ttu-id="1f606-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f606-109">Property</span></span>       | <span data-ttu-id="1f606-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f606-110">Type</span></span>              | <span data-ttu-id="1f606-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f606-111">Description</span></span>                           |
| :------------- | :---------------- | :------------------------------------ |
| <span data-ttu-id="1f606-112">uiElementnames</span><span class="sxs-lookup"><span data-stu-id="1f606-112">uiElementNames</span></span> | <span data-ttu-id="1f606-113">String collection</span><span class="sxs-lookup"><span data-stu-id="1f606-113">String collection</span></span> | <span data-ttu-id="1f606-114">O nome do elemento de interface do usuário do rodapé a ser removido.</span><span class="sxs-lookup"><span data-stu-id="1f606-114">The name of the UI element of footer to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1f606-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f606-115">JSON representation</span></span>

<span data-ttu-id="1f606-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f606-116">The following is a JSON representation of the resource.</span></span>

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