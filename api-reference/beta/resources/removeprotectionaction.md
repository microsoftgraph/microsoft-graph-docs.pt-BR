---
title: tipo de recurso removeProtectionAction
description: Representa uma ação para remover a proteção do arquivo ou informações.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 63a539fe4366703aaeb7e6b16735bb0302951dd7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521142"
---
# <a name="removeprotectionaction-resource-type"></a><span data-ttu-id="38bb7-103">tipo de recurso removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="38bb7-103">removeProtectionAction resource type</span></span>

<span data-ttu-id="38bb7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="38bb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38bb7-105">Representa uma ação para remover a proteção do arquivo ou informações.</span><span class="sxs-lookup"><span data-stu-id="38bb7-105">Represents an action to remove protection from the file or information.</span></span> <span data-ttu-id="38bb7-106">As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) podem retornar o **removeProtectionAction** se a proteção for removida como resultado da atualização ou remoção do rótulo.</span><span class="sxs-lookup"><span data-stu-id="38bb7-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeProtectionAction** if protection is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="38bb7-107">A ação instrui o aplicativo de consumo a remover o elemento de interface do usuário específico que contém o cabeçalho de conteúdo aplicável anteriormente.</span><span class="sxs-lookup"><span data-stu-id="38bb7-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content header.</span></span> <span data-ttu-id="38bb7-108">A proteção deve ser removida por uma biblioteca de cliente, como o Microsoft Information Protection SDK, somente se o usuário de chamada tiver direitos suficientes para remover a proteção.</span><span class="sxs-lookup"><span data-stu-id="38bb7-108">Protection should be removed via a client library, such as the Microsoft Information Protection SDK, only if the calling user has sufficient rights to remove protection.</span></span>

## <a name="properties"></a><span data-ttu-id="38bb7-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38bb7-109">Properties</span></span>

<span data-ttu-id="38bb7-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38bb7-110">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38bb7-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38bb7-111">JSON representation</span></span>

<span data-ttu-id="38bb7-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38bb7-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeProtectionAction",
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
  "description": "removeProtectionAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->