---
title: tipo de recurso removeContentHeaderAction
description: Representa uma ação que especifica os detalhes no cabeçalho de conteúdo a ser removido das informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 63dc9556ace567f4505b40c1882bd56b087a7835
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073422"
---
# <a name="removecontentheaderaction-resource-type"></a><span data-ttu-id="bd4a4-103">tipo de recurso removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="bd4a4-103">removeContentHeaderAction resource type</span></span>

<span data-ttu-id="bd4a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd4a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd4a4-105">Representa uma ação que especifica os detalhes no cabeçalho de conteúdo a ser removido das informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="bd4a4-105">Represents an action that specifies the details on the content header to be removed from the information, if applicable.</span></span> <span data-ttu-id="bd4a4-106">As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) podem retornar o **removeContentHeaderAction** se o cabeçalho for removido como resultado da atualização ou remoção do rótulo.</span><span class="sxs-lookup"><span data-stu-id="bd4a4-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeContentHeaderAction** if the header is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="bd4a4-107">A ação instrui o aplicativo de consumo a remover o elemento de interface do usuário específico que contém o cabeçalho de conteúdo aplicável anteriormente.</span><span class="sxs-lookup"><span data-stu-id="bd4a4-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content header.</span></span>

## <a name="properties"></a><span data-ttu-id="bd4a4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bd4a4-108">Properties</span></span>

| <span data-ttu-id="bd4a4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd4a4-109">Property</span></span>       | <span data-ttu-id="bd4a4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd4a4-110">Type</span></span>              | <span data-ttu-id="bd4a4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd4a4-111">Description</span></span>                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| <span data-ttu-id="bd4a4-112">uiElementnames</span><span class="sxs-lookup"><span data-stu-id="bd4a4-112">uiElementNames</span></span> | <span data-ttu-id="bd4a4-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd4a4-113">String collection</span></span> | <span data-ttu-id="bd4a4-114">O nome do elemento de interface do usuário do cabeçalho a ser removido.</span><span class="sxs-lookup"><span data-stu-id="bd4a4-114">The name of the UI element of the header to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bd4a4-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bd4a4-115">JSON representation</span></span>

<span data-ttu-id="bd4a4-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bd4a4-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeContentHeaderAction",
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
  "description": "removeContentHeaderAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

