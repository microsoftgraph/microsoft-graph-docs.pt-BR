---
title: tipo de recurso educationAssignmentIndividualRecipient
description: Usado dentro da propriedade assignment.assignTo.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4d5f01d3532e6b0022c10947ea36b19c2152fb36409a27cf58898006f5f016ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202424"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a>tipo de recurso educationAssignmentIndividualRecipient

Namespace: microsoft.graph

Usado dentro da [propriedade assignment.assignTo.](educationassignment.md) Quando definido como lista de destinatários individuais, os alunos selecionados na classe receberão um objeto de envio quando a atribuição for publicada.

Esse recurso é uma subclasse [de educationAssignmentRecipient](educationassignmentrecipient.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|destinatários|String collection|Uma coleção de IDs dos destinatários.|

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


