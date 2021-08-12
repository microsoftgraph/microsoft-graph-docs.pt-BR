---
title: Tipo de recurso accessReviewScope
description: Representa as entidades que precisam ser revisadas em uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9194d0b07c2b24d37f811c2348ed7b4b1a8498e2f592b6a10d97dc212d180be9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54121442"
---
# <a name="accessreviewscope-resource-type"></a>Tipo de recurso accessReviewScope

Namespace: microsoft.graph

O **accessReviewScope** define quais entidades serão revisadas em [accessReviewScheduleDefinition](accessreviewscheduledefinition.md). É um tipo abstrato herdado por [accessReviewQueryScope](accessreviewqueryscope.md), [principalResourceMembershipsScope](principalresourcemembershipsscope.md) e [accessReviewReviewerScope](accessreviewreviewerscope.md). 

Para **a propriedade scope** em um [accessReviewScheduleDefinition,](accessreviewscheduledefinition.md) consulte [accessReviewQueryScope](accessreviewqueryscope.md) e [principalResourceMembershipsScope](principalresourcemembershipsscope.md).

Para **a propriedade reviewers** em [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md) consulte [accessReviewReviewerScope](accessreviewreviewerscope.md).

A especificação do tipo  OData no escopo é altamente recomendada para todos os tipos, mas necessária para [o principalResourceMembershipsScope](principalresourcemembershipsscope.md) e [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).

## <a name="properties"></a>Propriedades
Nenhum.


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScope"
}
```
