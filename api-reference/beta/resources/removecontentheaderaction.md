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
# <a name="removecontentheaderaction-resource-type"></a>tipo de recurso removeContentHeaderAction

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma ação que especifica os detalhes no cabeçalho de conteúdo a ser removido das informações, se aplicável. As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) podem retornar o **removeContentHeaderAction** se o cabeçalho for removido como resultado da atualização ou remoção do rótulo. A ação instrui o aplicativo de consumo a remover o elemento de interface do usuário específico que contém o cabeçalho de conteúdo aplicável anteriormente.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo              | Descrição                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| uiElementnames | String collection | O nome do elemento de interface do usuário do cabeçalho a ser removido. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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