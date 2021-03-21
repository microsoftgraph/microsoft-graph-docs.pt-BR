---
title: Tipo de recurso removeProtectionAction
description: Representa uma ação para remover a proteção do arquivo ou informações.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2b315c9d2641524d8a134f0e0b9704c51419ada4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962032"
---
# <a name="removeprotectionaction-resource-type"></a><span data-ttu-id="eb640-103">Tipo de recurso removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="eb640-103">removeProtectionAction resource type</span></span>

<span data-ttu-id="eb640-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb640-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb640-105">Representa uma ação para remover a proteção do arquivo ou informações.</span><span class="sxs-lookup"><span data-stu-id="eb640-105">Represents an action to remove protection from the file or information.</span></span> <span data-ttu-id="eb640-106">As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) podem retornar as APIs **removeProtectionAction** se a proteção for removida como resultado da atualização ou remoção do rótulo.</span><span class="sxs-lookup"><span data-stu-id="eb640-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeProtectionAction** if protection is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="eb640-107">A ação instrui o aplicativo de consumo a remover o elemento de interface do usuário específico que contém o header de conteúdo anteriormente aplicável.</span><span class="sxs-lookup"><span data-stu-id="eb640-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content header.</span></span> <span data-ttu-id="eb640-108">A proteção deve ser removida por meio de uma biblioteca de clientes, como o SDK da Proteção de Informações da Microsoft, somente se o usuário de chamada tiver direitos suficientes para remover a proteção.</span><span class="sxs-lookup"><span data-stu-id="eb640-108">Protection should be removed via a client library, such as the Microsoft Information Protection SDK, only if the calling user has sufficient rights to remove protection.</span></span>

## <a name="properties"></a><span data-ttu-id="eb640-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb640-109">Properties</span></span>

<span data-ttu-id="eb640-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb640-110">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb640-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb640-111">JSON representation</span></span>

<span data-ttu-id="eb640-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb640-112">The following is a JSON representation of the resource.</span></span>

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

