---
title: Tipo de recurso decisionItemPrincipalResourceMembership
description: Cada decisão em uma revisão de acesso representa o acesso de uma entidade de segurança a um recurso. Um objeto decisionItemPrincipalResourceMembership expõe os detalhes do tipo de associação que a entidade de segurança tem ao recurso associado ao objeto accessReviewInstanceDecisionItem.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: eed87ba5ad700330c1c2449060e9397c8eb6408c
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698258"
---
# <a name="decisionitemprincipalresourcemembership-resource-type"></a>Tipo de recurso decisionItemPrincipalResourceMembership

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Cada decisão em uma revisão de acesso representa o acesso de uma entidade de segurança a um recurso. Um **objeto decisionItemPrincipalResourceMembership** expõe os detalhes do tipo de associação que a entidade de segurança tem ao recurso associado ao objeto [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) . Por exemplo, a entidade de segurança pode ter acesso direto ou indireto ao recurso.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|membershipType| decisionItemPrincipalResourceMembershipType | Tipo de associação que a entidade de segurança tem ao recurso. Com valores múltiplos. Os valores possíveis são: `direct`, `indirect`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.decisionItemPrincipalResourceMembership",
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.decisionItemPrincipalResourceMembership",
  "membershipType": "String",
}
```
