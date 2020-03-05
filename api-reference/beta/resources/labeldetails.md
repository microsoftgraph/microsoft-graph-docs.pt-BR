---
title: tipo de recurso labelDetails
description: Representa os detalhes do rótulo de um rótulo de proteção de informações.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cf031459004e0c0d56b5b09145ed897a9f960142
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523006"
---
# <a name="labeldetails-resource-type"></a>tipo de recurso labelDetails

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes do rótulo de um rótulo de proteção de informações. **labelDetails** fornece informações sobre um único rótulo de proteção de informações. Pode ser retornado por [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)e [extractLabel](../api/informationprotectionlabel-extractLabel.md)

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo    | Descrição                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| color       | String  | A cor que a interface do usuário deve exibir para o rótulo, se configurada.                               |
| description | Cadeia de caracteres  | A descrição definida pelo administrador para o rótulo.                                                                 |
| id          | String  | A ID do rótulo é um identificador global exclusivo (GUID).                                                          |
| isActive    | Boolean | Indica se o rótulo está ativo ou não. Os rótulos ativos devem ser ocultos ou desabilitados nas interfaces de usuário. |
| nome        | Cadeia de caracteres  | O nome de texto não criptografado do rótulo.                                                                             |
| sensitivity | Int32   | O valor de confidencialidade do rótulo, onde inferior é menos confidencial.                                           |
| tooltip     | String  | A dica de ferramenta que deve ser exibida para o rótulo em uma interface de usuário.                                      |

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