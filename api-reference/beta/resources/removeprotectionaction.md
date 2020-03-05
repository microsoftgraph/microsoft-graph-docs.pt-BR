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
# <a name="removeprotectionaction-resource-type"></a>tipo de recurso removeProtectionAction

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma ação para remover a proteção do arquivo ou informações. As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) podem retornar o **removeProtectionAction** se a proteção for removida como resultado da atualização ou remoção do rótulo. A ação instrui o aplicativo de consumo a remover o elemento de interface do usuário específico que contém o cabeçalho de conteúdo aplicável anteriormente. A proteção deve ser removida por uma biblioteca de cliente, como o Microsoft Information Protection SDK, somente se o usuário de chamada tiver direitos suficientes para remover a proteção.

## <a name="properties"></a>Propriedades

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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