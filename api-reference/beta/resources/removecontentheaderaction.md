---
title: tipo de recurso removeContentHeaderAction
description: Representa uma ação que especifica os detalhes no cabeçalho de conteúdo a ser removido das informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 907113e20b5e4257a672190433efd055a628c17f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521149"
---
# <a name="removecontentheaderaction-resource-type"></a><span data-ttu-id="4a7b5-103">tipo de recurso removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="4a7b5-103">removeContentHeaderAction resource type</span></span>

<span data-ttu-id="4a7b5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4a7b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a7b5-105">Representa uma ação que especifica os detalhes no cabeçalho de conteúdo a ser removido das informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="4a7b5-105">Represents an action that specifies the details on the content header to be removed from the information, if applicable.</span></span> <span data-ttu-id="4a7b5-106">As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) podem retornar o **removeContentHeaderAction** se o cabeçalho for removido como resultado da atualização ou remoção do rótulo.</span><span class="sxs-lookup"><span data-stu-id="4a7b5-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeContentHeaderAction** if the header is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="4a7b5-107">A ação instrui o aplicativo de consumo a remover o elemento de interface do usuário específico que contém o cabeçalho de conteúdo aplicável anteriormente.</span><span class="sxs-lookup"><span data-stu-id="4a7b5-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content header.</span></span>

## <a name="properties"></a><span data-ttu-id="4a7b5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a7b5-108">Properties</span></span>

| <span data-ttu-id="4a7b5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a7b5-109">Property</span></span>       | <span data-ttu-id="4a7b5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a7b5-110">Type</span></span>              | <span data-ttu-id="4a7b5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a7b5-111">Description</span></span>                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| <span data-ttu-id="4a7b5-112">uiElementnames</span><span class="sxs-lookup"><span data-stu-id="4a7b5-112">uiElementNames</span></span> | <span data-ttu-id="4a7b5-113">String collection</span><span class="sxs-lookup"><span data-stu-id="4a7b5-113">String collection</span></span> | <span data-ttu-id="4a7b5-114">O nome do elemento de interface do usuário do cabeçalho a ser removido.</span><span class="sxs-lookup"><span data-stu-id="4a7b5-114">The name of the UI element of the header to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4a7b5-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a7b5-115">JSON representation</span></span>

<span data-ttu-id="4a7b5-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a7b5-116">The following is a JSON representation of the resource.</span></span>

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