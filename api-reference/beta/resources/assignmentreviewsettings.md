---
title: tipo de recurso assignmentReviewSettings
description: O tipo assignmentReviewSettings, usado para a propriedade accessReviewSettings de uma política de atribuição de pacote do Access, fornece configurações adicionais para selecionar quem deve revisar as atribuições de pacote de acesso desta política e com que frequência elas devem ser revisadas.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c673d96ab5bb6dbb6f217d5b36f41520b421f5bf
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331345"
---
# <a name="assignmentreviewsettings-resource-type"></a>tipo de recurso assignmentReviewSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para a propriedade **accessReviewSettings** de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md). Fornece configurações adicionais para selecionar quem deve revisar as atribuições de pacote de acesso desta política e com que frequência elas devem ser revisadas.  

## <a name="properties"></a>Propriedades

Este tipo tem as seguintes propriedades:

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| isEnabled| Boolean | Se verdadeiro, as revisões do Access são necessárias para as atribuições desta política. |
| recurrenceType | String | O intervalo de recorrência, como `monthly` ou `quarterly`. |
| revisor | String | Quem deve ser solicitado a fazer a revisão, `Self` ou. `Reviewers` |
| startDateTime | DateTimeOffset | Quando a primeira revisão deve iniciar. |
| durationInDays | Int32 | O número de dias para permitir a entrada de revisores.|
| revisores | coleção [userset](userset.md) | Se o revisortype for `Reviewers`, essa coleção especifica os usuários que serão revisores, por ID ou como membros de um grupo, usando uma coleção de [únicousuário](singleuser.md) e [groupMembers](groupmembers.md). |

## <a name="json-representation"></a>Representação JSON


Veja a seguir uma representação JSON da propriedade de configurações de revisão do Access de uma política.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignmentReviewSettings",
  "baseType": ""
}-->

```json
{
  "isEnabled": true,
  "recurrenceType": "quarterly",
  "reviewerType": "Self",
  "startDateTime": "2020-01-23T07:59:59.998Z",
  "durationInDays": 25,
  "reviewers": []
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignmentReviewSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
