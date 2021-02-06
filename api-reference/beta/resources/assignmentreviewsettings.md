---
title: Tipo de recurso assignmentReviewSettings
description: O tipo assignmentReviewSettings, usado para a propriedade accessReviewSettings de uma política de atribuição de pacote de acesso, fornece configurações adicionais para selecionar quem deve revisar as atribuições de pacote de acesso dessa política e com que frequência elas devem ser revisadas.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bde8c6d330eda7e100071edbf2190e170ca913ea
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131318"
---
# <a name="assignmentreviewsettings-resource-type"></a>Tipo de recurso assignmentReviewSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para a **propriedade accessReviewSettings** de uma política [de atribuição de pacote de acesso.](accesspackageassignmentpolicy.md) Fornece configurações adicionais para selecionar quem deve revisar as atribuições do pacote de acesso desta política e a frequência com que elas devem ser revisadas.  

## <a name="properties"></a>Propriedades

Esse tipo tem as seguintes propriedades:

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| isEnabled| Booliano | Se for verdadeiro, as revisões de acesso serão necessárias para as atribuições dessa política. |
| recurrenceType | String | O intervalo de recorrência, como `monthly` ou `quarterly` . |
| reviewerType | String | Quem deve ser solicitado a fazer a revisão, `Self` ou `Reviewers` . |
| startDateTime | DateTimeOffset | Quando a primeira revisão deve começar. |
| durationInDays | Int32 | O número de dias para permitir a entrada dos revisadores.|
| reviewers | [Coleção userSet](userset.md) | Se reviewerType for , esta coleção especificará os usuários que serão revisadores, por ID ou como membros de um grupo, usando uma coleção de `Reviewers` [singleUser](singleuser.md) e [groupMembers](groupmembers.md). |

## <a name="json-representation"></a>Representação JSON


A seguir está uma representação JSON da propriedade de configurações de revisão de acesso de uma política.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignmentReviewSettings"
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


