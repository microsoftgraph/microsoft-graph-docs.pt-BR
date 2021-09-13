---
title: tipo de recurso educationAssignmentIndividualRecipient
description: Usado dentro da propriedade assignment.assignTo.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5e8038aafd8271ffbd4dc92b12fd236c1f7a9923
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109139"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a>tipo de recurso educationAssignmentIndividualRecipient

Namespace: microsoft.graph

Usado dentro da [propriedade assignment.assignTo.](educationassignment.md) Quando definido como lista de destinatários individuais, os alunos selecionados na classe receberão um objeto de envio quando a atribuição for publicada.

Esse recurso é uma subclasse [de educationAssignmentRecipient](educationassignmentrecipient.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|destinatários|Coleção String|Uma coleção de IDs dos destinatários.|

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


