---
title: Tipo de recurso removeContentFooterAction
description: Representa uma ação que especifica os detalhes no rodapé de conteúdo a serem removidos das informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1e8de130b2ad346e8e1fee2077014eda9e9b94d5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962068"
---
# <a name="removecontentfooteraction-resource-type"></a>Tipo de recurso removeContentFooterAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma ação que especifica os detalhes no rodapé de conteúdo a serem removidos das informações, se aplicável. As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) podem retornar **o removeContentFooterAction** se o rodapé for removido como resultado da atualização ou remoção do rótulo. A ação instrui o aplicativo de consumo a remover o elemento de interface do usuário específico que contém o rodapé de conteúdo anteriormente aplicável.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo              | Descrição                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| uiElementNames | Coleção de cadeias de caracteres | O nome do elemento de interface do usuário do rodapé a ser removido. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeContentFooterAction",
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
  "description": "removeContentFooterAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

