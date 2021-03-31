---
title: Tipo de recurso accessReviewInactiveUsersQueryScope
description: Um tipo de accessReviewQueryScope que permite que apenas usuários inativos sejam selecionados no escopo de uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 51fc61ce186b0346bc065ddc5dfea40158758223
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469732"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a>Tipo de recurso accessReviewInactiveUsersQueryScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Um tipo de [accessReviewQueryScope](../resources/accessreviewqueryscope.md) que permite que apenas usuários inativos sejam selecionados no escopo de uma revisão de acesso.

Herda de [accessReviewQueryScope](../resources/accessreviewqueryscope.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|inactiveDuration|Duration|Define o comprimento do período de duração da inatividade. A inatividade é baseada na última data de login do usuário.|
|consulta|String|Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).|
|queryRoot|String|Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).|
|queryType|String|Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).|

### <a name="supported-queries-for-accessreviewinactiveuserqueryscope-as-scope"></a>Consultas com suporte para accessReviewInactiveUserQueryScope como escopo
As mesmas consultas com suporte no [accessReviewScope](../resources/accessreviewscope.md) também são suportadas no accessReviewInactiveUserQueryScope. A seguir estão as consultas. Eles são suportados como a `scope` propriedade em [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).

|Cenário| Consulta |
|--|--|
| Revisar todos os usuários convidados inativos atribuídos a um grupo | /groups/{group ID}/transitiveMembers/microsoft.graph.user/? \$ count=true&$filter=(userType eq 'Guest') |
| Revisar todos os usuários inativos atribuídos a um grupo | /groups/{group ID}/transitiveMembers |
| Revisar todos os usuários convidados inativos atribuídos a todos os grupos | ./members/microsoft.graph.user/? \$ count=true&$filter=(userType eq 'Guest') |


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInactiveUsersQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String",
  "inactiveDuration": "String (duration)"
}
```
