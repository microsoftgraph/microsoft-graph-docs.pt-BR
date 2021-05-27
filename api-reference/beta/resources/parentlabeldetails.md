---
title: Tipo de recurso parentLabelDetails
description: Representa os detalhes do rótulo de um rótulo pai de proteção de informações.
localization_priority: Normal
author: tommoser
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8f1ebe58c3968e0f912806eb6f339bcfd499b57a
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679895"
---
# <a name="parentlabeldetails-resource-type"></a>Tipo de recurso parentLabelDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes do rótulo de um rótulo pai de proteção de informações. **parentLabelDetails** fornece informações sobre um único rótulo de proteção de informações. Pode ser retornado [por evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)e [extractLabel](../api/informationprotectionlabel-extractLabel.md)

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo    | Descrição                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| color       | String  | A cor que a interface do usuário deve exibir para o rótulo, se configurada.                               |
| descrição | String  | A descrição definida pelo administrador para o rótulo.                                                                 |
| id          | String  | A ID do rótulo é um identificador global exclusivo (GUID).                                                          |
| isActive    | Boolean | Indica se o rótulo está ativo ou não. Os rótulos ativos devem ser ocultos ou desabilitados nas interfaces do usuário. |
| nome        | String  | O nome do texto sem formatção do rótulo.                                                                             |
| sensitivity | Int32   | O valor de sensibilidade do rótulo, onde menor é menos sensível.                                           |
| tooltip     | String  | A dica de ferramenta que deve ser exibida para o rótulo em uma interface do usuário.                                      |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.parentLabelDetails",
  "baseType": null
}-->

```json
{
  "color": "String",
  "description": "String",
  "id": "String",
  "isActive": true,
  "name": "String",
  "sensitivity": 1024,
  "tooltip": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "parentLabelDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->