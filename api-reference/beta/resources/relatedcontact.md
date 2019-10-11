---
title: tipo de recurso relatedContact
description: Registro de contato relacionado a um educationUser que fornece informações para guardiões, auxílios, médicos e assim por diante.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ce1ff84abb6704255267b521c67e5fc7b231b7df
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439931"
---
# <a name="relatedcontact-resource-type"></a>tipo de recurso relatedContact

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Registro de contato relacionado a um [educationUser](../resources/educationuser.md) que fornece informações para guardiões, auxílios, médicos e assim por diante.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                  | Descrição                                                                                                         |
| :------------ | :-------------------- | :------------------------------------------------------------------------------------------------------------------ |
| id            | Cadeia de caracteres                | Identidade do contato no Azure Active Directory.                                                              |
| displayName   | Cadeia de caracteres                | Nome do contato. Obrigatório.                                                                                      |
| emailAddress  | String                | Endereço de email principal do contato.                                                                               |
| mobilePhone   | String                | Número do telefone celular do contato.                                                                                 |
| relação  | `contactRelationship` | Relação com o usuário. Os valores possíveis `parent`são `relative`: `aide` `doctor` `guardian`,,, `child`, `other`,. |
| accessConsent | Booliano               | Indica se o usuário foi remetido para acessar os dados dos alunos.                                               |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedContact"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "contactRelationship",
  "accessConsent": true
}
```

<!-- uuid: 720F9AB6-6E7A-4A66-8B0A-37A556FF99C5
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "relatedContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
