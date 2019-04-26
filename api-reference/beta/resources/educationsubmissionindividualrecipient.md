---
title: tipo de recurso educationSubmissionIndividualRecipient
description: 'Uma subclasse de educationSubmissionRecipient que indica que um envio é atribuído a um indivíduo na classe.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: de58dc743cd50f0e31021b4651bb0a3b3b192197
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340532"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a>tipo de recurso educationSubmissionIndividualRecipient

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma subclasse de [educationSubmissionRecipient](educationsubmissionrecipient.md) que indica que um envio é atribuído a um indivíduo na classe.  


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|userId|Cadeia de caracteres|ID de usuário do usuário para o qual o envio é atribuído.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionIndividualRecipient"
}-->

```json
{
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
