---
title: tipo de recurso educationAssignmentIndividualRecipient
description: 'Usada dentro da propriedade assignment. assignTo. Quando definido como lista de destinatários individuais, os alunos selecionados na classe serão '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 39d3fb4875412546cd6f182de05ad1779b05abdd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334408"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a>tipo de recurso educationAssignmentIndividualRecipient

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usada dentro da propriedade [assignment.](educationassignment.md) assignTo. Quando definido como lista de destinatários individuais, os alunos selecionados na classe receberão um objeto de envio quando a atribuição for publicada.

Esse recurso é uma subclasse de [educationAssignmentRecipient](educationassignmentrecipient.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recipients|Coleção String|Uma coleção de IDs dos destinatários.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentIndividualRecipient"
}-->

```json
{
  "recipients": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
