---
title: Tipo de recurso accessReviewScope
description: Representa as entidades que precisam ser revisadas em uma revisão de acesso.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f14589faad21b586fb3dcc2c6f8b16be9da84f03
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698426"
---
# <a name="accessreviewscope-resource-type"></a>Tipo de recurso accessReviewScope

Namespace: microsoft.graph

O **accessReviewScope** define quais entidades são revisadas em [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md). É um tipo abstrato herdado por [accessReviewQueryScope](accessreviewqueryscope.md), [principalResourceMembershipsScope](principalresourcemembershipsscope.md) e [accessReviewReviewerScope](accessreviewreviewerscope.md). 

Para **obter** a propriedade scope em [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md) , consulte [accessReviewQueryScope](accessreviewqueryscope.md) e [principalResourceMembershipsScope](principalresourcemembershipsscope.md).

Para **a propriedade** reviewers em [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md) , [consulte accessReviewReviewerScope](accessreviewreviewerscope.md).

Especificar o tipo OData no escopo é  altamente recomendável para todos os tipos, mas necessário para [principalResourceMembershipsScope](principalresourcemembershipsscope.md) e [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).

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
