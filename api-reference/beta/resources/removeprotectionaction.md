---
title: tipo de recurso removeProtectionAction
description: Representa uma ação para remover a proteção do arquivo ou informações.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b3ed559460947e903e3085ab48edb421045bc3c6
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939275"
---
# <a name="removeprotectionaction-resource-type"></a><span data-ttu-id="10d9a-103">tipo de recurso removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="10d9a-103">removeProtectionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10d9a-104">Representa uma ação para remover a proteção do arquivo ou informações.</span><span class="sxs-lookup"><span data-stu-id="10d9a-104">Represents an action to remove protection from the file or information.</span></span> <span data-ttu-id="10d9a-105">As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) podem retornar o **removeProtectionAction** se a proteção for removida como resultado da atualização ou remoção do rótulo.</span><span class="sxs-lookup"><span data-stu-id="10d9a-105">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeProtectionAction** if protection is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="10d9a-106">A ação instrui o aplicativo de consumo a remover o elemento de interface do usuário específico que contém o cabeçalho de conteúdo aplicável anteriormente.</span><span class="sxs-lookup"><span data-stu-id="10d9a-106">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content header.</span></span> <span data-ttu-id="10d9a-107">A proteção deve ser removida por uma biblioteca de cliente, como o Microsoft Information Protection SDK, somente se o usuário de chamada tiver direitos suficientes para remover a proteção.</span><span class="sxs-lookup"><span data-stu-id="10d9a-107">Protection should be removed via a client library, such as the Microsoft Information Protection SDK, only if the calling user has sufficient rights to remove protection.</span></span>

## <a name="properties"></a><span data-ttu-id="10d9a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10d9a-108">Properties</span></span>

<span data-ttu-id="10d9a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10d9a-109">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10d9a-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10d9a-110">JSON representation</span></span>

<span data-ttu-id="10d9a-111">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10d9a-111">The following is a JSON representation of the resource.</span></span>

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