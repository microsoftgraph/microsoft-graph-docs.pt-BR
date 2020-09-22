---
title: tipo de recurso removeProtectionAction
description: Representa uma ação para remover a proteção do arquivo ou informações.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bf4ad367038367d3572f0451bfa7d3eb0a25368d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073394"
---
# <a name="removeprotectionaction-resource-type"></a><span data-ttu-id="e6ca2-103">tipo de recurso removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="e6ca2-103">removeProtectionAction resource type</span></span>

<span data-ttu-id="e6ca2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6ca2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6ca2-105">Representa uma ação para remover a proteção do arquivo ou informações.</span><span class="sxs-lookup"><span data-stu-id="e6ca2-105">Represents an action to remove protection from the file or information.</span></span> <span data-ttu-id="e6ca2-106">As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) podem retornar o **removeProtectionAction** se a proteção for removida como resultado da atualização ou remoção do rótulo.</span><span class="sxs-lookup"><span data-stu-id="e6ca2-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeProtectionAction** if protection is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="e6ca2-107">A ação instrui o aplicativo de consumo a remover o elemento de interface do usuário específico que contém o cabeçalho de conteúdo aplicável anteriormente.</span><span class="sxs-lookup"><span data-stu-id="e6ca2-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content header.</span></span> <span data-ttu-id="e6ca2-108">A proteção deve ser removida por uma biblioteca de cliente, como o Microsoft Information Protection SDK, somente se o usuário de chamada tiver direitos suficientes para remover a proteção.</span><span class="sxs-lookup"><span data-stu-id="e6ca2-108">Protection should be removed via a client library, such as the Microsoft Information Protection SDK, only if the calling user has sufficient rights to remove protection.</span></span>

## <a name="properties"></a><span data-ttu-id="e6ca2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6ca2-109">Properties</span></span>

<span data-ttu-id="e6ca2-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6ca2-110">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6ca2-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6ca2-111">JSON representation</span></span>

<span data-ttu-id="e6ca2-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6ca2-112">The following is a JSON representation of the resource.</span></span>

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

