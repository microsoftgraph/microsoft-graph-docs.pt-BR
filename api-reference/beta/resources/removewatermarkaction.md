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
# <a name="removewatermarkaction-resource-type"></a>tipo de recurso removeWatermarkAction

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma ação que especifica os detalhes sobre a marca d' água de conteúdo a ser removido das informações, se aplicável. As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) podem retornar o **removeWatermarkAction** se a marca d' água for removida como resultado da atualização ou remoção do rótulo. A ação instrui o aplicativo de consumo a remover o elemento de interface do usuário específico que contém a marca d' água de conteúdo aplicável anteriormente.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo              | Descrição                           |
| :------------- | :---------------- | :------------------------------------ |
| uiElementnames | String collection | O nome do elemento de interface do usuário do rodapé a ser removido. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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