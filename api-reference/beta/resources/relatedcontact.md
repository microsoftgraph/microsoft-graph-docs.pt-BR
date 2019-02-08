---
title: tipo de recurso de relatedContact
description: Registro de contato relacionado a um educationUser que fornece informações para responsáveis, auxílios, os médicos e assim por diante.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d29cf93154e2c032ac7010372e3f116f2a1dd46c
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2019
ms.locfileid: "29694472"
---
# <a name="relatedcontact-resource-type"></a>tipo de recurso de relatedContact

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Entre em contato com o registro de um [educationUser](../resources/educationuser.md) que fornece informações para responsáveis, auxílios, os médicos e assim por diante.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String|Identidade do contato dentro do Azure Active Directory.|
|displayName|String|Nome do contato. Obrigatório.|
|emailAddress|String|Endereço de email principal do contato.|
|mobilePhone|String|Número de telefone celular do contato.|
|Relação|`contactRelationship`|Relacionamento ao usuário. Os valores possíveis são `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.|
|accessConsent|Boolean|Indica se o usuário foi aceitou para acessar dados de student.|

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
