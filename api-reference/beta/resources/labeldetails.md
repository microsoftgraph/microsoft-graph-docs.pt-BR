---
title: Tipo de recurso labelDetails
description: Representa os detalhes do rótulo de um rótulo de proteção de informações.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: eb66e395d18b7887942753abdebd91d398844290
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579288"
---
# <a name="labeldetails-resource-type"></a>Tipo de recurso labelDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes do rótulo de um rótulo de proteção de informações. **labelDetails** fornece informações sobre um único rótulo de proteção de informações. Herda do [parentLabelDetails](parentlabeldetails.md). Pode ser retornado [por evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)e [extractLabel](../api/informationprotectionlabel-extractLabel.md)

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo                                         | Descrição                                                                                                  |
| :---------- | :------------------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| color       | String                                       | A cor que a interface do usuário deve exibir para o rótulo, se configurada.                               |
| descrição | String                                       | A descrição definida pelo administrador para o rótulo.                                                                 |
| id          | String                                       | A ID do rótulo é um identificador global exclusivo (GUID).                                                         |
| isActive    | Booliano                                      | Indica se o rótulo está ativo ou não. Os rótulos ativos devem ser ocultos ou desabilitados nas interfaces do usuário. |
| nome        | String                                       | O nome do texto sem formatção do rótulo.                                                                             |
| sensitivity | Int32                                        | O valor de sensibilidade do rótulo, onde menor é menos sensível.                                           |
| tooltip     | String                                       | A dica de ferramenta que deve ser exibida para o rótulo em uma interface do usuário.                                      |
| primário      | parentLabelDetails | O rótulo pai associado a um rótulo filho.                                                              |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.labelDetails",
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
  "description": "labelDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

