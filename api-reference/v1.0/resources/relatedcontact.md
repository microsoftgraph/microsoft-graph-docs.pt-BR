---
title: tipo de recurso relatedContact
description: Registro de contato relacionado a um educationUser que fornece informações para tutores, auxiliares, médicos e assim por diante.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 528244c6cc84ab26c21ec1ea5c15c7bc8e68c082
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59035994"
---
# <a name="relatedcontact-resource-type"></a>tipo de recurso relatedContact

Namespace: microsoft.graph

Registro de contato relacionado a [um educationUser](../resources/educationuser.md) que fornece informações para tutores, auxiliares, médicos e assim por diante.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                  | Descrição                                                                                                                               |
| :------------ | :-------------------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| id            | Cadeia de caracteres                | Identidade do contato dentro Azure Active Directory.                                                                                    |
| displayName   | Cadeia de caracteres                | Nome do contato. Obrigatório.                                                                                                            |
| emailAddress  | String                | Endereço de email principal do contato.                                                                                                     |
| mobilePhone   | String                | Número de telefone celular do contato.                                                                                                       |
| relação  | `contactRelationship` | Relação com o usuário. Os valores possíveis `parent` são , , , , , , , `relative` `aide` `doctor` `guardian` `child` `other` `unknownFutureValue` . |
| accessConsent | Booliano               | Indica se o usuário foi consentido para acessar dados de alunos.                                                                     |

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

