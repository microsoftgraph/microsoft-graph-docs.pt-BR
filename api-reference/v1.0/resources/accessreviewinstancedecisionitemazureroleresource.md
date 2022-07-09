---
title: Tipo de recurso accessReviewInstanceDecisionItemAzureRoleResource
description: Representa as funções de recurso do Azure para as quais o acesso é representado por meio de um objeto accessReviewInstanceDecisionItem.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b1b8e2c671c65c9efc97014b5614c585c7c1c37e
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698286"
---
# <a name="accessreviewinstancedecisionitemazureroleresource-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItemAzureRoleResource

Namespace: microsoft.graph

Representa as funções de recurso do Azure para as quais o acesso é representado por meio de um [objeto accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) . **accessReviewInstanceDecisionItemAzureRoleResource** é um tipo aberto que permite que outras propriedades sejam passadas.

Herda de [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| displayName | Cadeia de caracteres | Nome de exibição da função do Azure. Herdado [de accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).|
| id | Cadeia de caracteres | Identificador do recurso do item de decisão. Herdado [de accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |
| type | Cadeia de caracteres | Tipo de recurso. O tipo sempre será `AzureRole`.  Herdado [de accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |
| scope | [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md) | Detalhes do escopo ao qual essa função está associada. |


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",
  "baseType": "microsoft.graph.accessReviewInstanceDecisionItemResource",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String",
  "scope": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
  }
}
```
