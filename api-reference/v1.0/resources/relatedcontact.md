---
title: tipo de recurso relatedContact
description: Registro de contato relacionado a um educationUser que fornece informações para guardiões, auxílios, médicos e assim por diante.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 93069c2f9f2aa46c5d6d0f2f992762efab062064
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533865"
---
# <a name="realtedcontact-resource-type"></a>tipo de recurso realtedContact

Namespace: microsoft.graph

Registro de contato relacionado a um [educationUser](../resources/educationuser.md) que fornece informações para guardiões, auxílios, médicos e assim por diante.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String|Identidade do contato no Azure Active Directory.|
|displayName|Cadeia de caracteres|Nome do contato. Obrigatório.|
|emailAddress|String|Endereço de email principal do contato.|
|mobilePhone|String|Número do telefone celular do contato.|
|relação|`contactRelationship`|Relação com o usuário. Os valores possíveis `parent`são `relative`: `aide` `doctor` `guardian` `child`,,,, `other`, `unknownFutureValue`,.|
|accessConsent|Booliano|Indica se o usuário foi remetido para acessar os dados dos alunos.|

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
