---
title: tipo de recurso relatedContact
description: Registro de contato relacionado a um educationUser que fornece informações para guardiões, auxílios, médicos e assim por diante.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: adea95729dd4e6558885223245a7225811f14677
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002944"
---
# <a name="realtedcontact-resource-type"></a>tipo de recurso realtedContact

Namespace: microsoft.graph

Registro de contato relacionado a um [educationUser](../resources/educationuser.md) que fornece informações para guardiões, auxílios, médicos e assim por diante.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                  | Descrição                                                                                                                               |
| :------------ | :-------------------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| id            | String                | Identidade do contato no Azure Active Directory.                                                                                    |
| displayName   | String                | Nome do contato. Obrigatório.                                                                                                            |
| emailAddress  | String                | Endereço de email principal do contato.                                                                                                     |
| mobilePhone   | String                | Número do telefone celular do contato.                                                                                                       |
| relação  | `contactRelationship` | Relação com o usuário. Os valores possíveis são:,,,,, `parent` `relative` `aide` `doctor` `guardian` `child` `other` , `unknownFutureValue` . |
| accessConsent | Boolean               | Indica se o usuário foi remetido para acessar os dados dos alunos.                                                                     |

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

