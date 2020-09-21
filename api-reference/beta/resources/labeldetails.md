---
title: tipo de recurso labelDetails
description: Representa os detalhes do rótulo de um rótulo de proteção de informações.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6b475c96b3ecbc2caa0aa147e3fc8fd0253ac243
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084034"
---
# <a name="labeldetails-resource-type"></a>tipo de recurso labelDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes do rótulo de um rótulo de proteção de informações. **labelDetails** fornece informações sobre um único rótulo de proteção de informações. Pode ser retornado por [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)e [extractLabel](../api/informationprotectionlabel-extractLabel.md)

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo    | Descrição                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| color       | String  | A cor que a interface do usuário deve exibir para o rótulo, se configurada.                               |
| description | Cadeia de caracteres  | A descrição definida pelo administrador para o rótulo.                                                                 |
| id          | Cadeia de caracteres  | A ID do rótulo é um identificador global exclusivo (GUID).                                                          |
| isActive    | Boolean | Indica se o rótulo está ativo ou não. Os rótulos ativos devem ser ocultos ou desabilitados nas interfaces de usuário. |
| name        | Cadeia de caracteres  | O nome de texto não criptografado do rótulo.                                                                             |
| sensitivity | Int32   | O valor de confidencialidade do rótulo, onde inferior é menos confidencial.                                           |
| tooltip     | Cadeia de caracteres  | A dica de ferramenta que deve ser exibida para o rótulo em uma interface de usuário.                                      |

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

