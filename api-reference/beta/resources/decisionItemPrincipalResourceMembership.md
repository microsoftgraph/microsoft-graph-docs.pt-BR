---
title: Tipo de recurso decisionItemPrincipalResourceMembership
description: Cada decisão em uma revisão de acesso representa o acesso de uma entidade de segurança a um recurso. Um objeto decisionItemPrincipalResourceMembership expõe os detalhes do tipo de associação que a entidade de segurança tem ao recurso associado ao objeto accessReviewInstanceDecisionItem.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9ff76ae47d8289827b9c6309288272d3b9c1e6c1
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447504"
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
