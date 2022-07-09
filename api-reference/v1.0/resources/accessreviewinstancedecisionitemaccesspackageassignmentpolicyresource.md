---
title: Tipo de recurso accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource
description: Representa uma política de atribuição de pacote de acesso para a qual o acesso é representado por meio de um objeto accessReviewInstanceDecisionItem.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 40cbb74fd9a9801b62f4a98809d28c56dbc86b2e
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698300"
---
# <a name="accessreviewinstancedecisionitemaccesspackageassignmentpolicyresource-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource

Namespace: microsoft.graph

Representa uma política de atribuição de pacote de acesso para a qual o acesso é representado por meio de um [objeto accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) . **accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource** é um tipo aberto que permite que outras propriedades sejam passadas.

Herda de [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|accessPackageDisplayName|Cadeia de caracteres| Nome de exibição do pacote de acesso ao qual o acesso foi concedido. |
|accessPackageId|Cadeia de caracteres| Identificador do pacote de acesso ao qual o acesso foi concedido. |
| displayName | Cadeia de caracteres | Nome de exibição do pacote de acesso. Herdado [de accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).|
| id | Cadeia de caracteres | Identificador do recurso do item de decisão. Herdado [de accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |
| type | Cadeia de caracteres | Tipo de recurso. O tipo sempre será `AccessPackageAssignmentPolicy`.  Herdado [de accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |



## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource",
  "baseType": "microsoft.graph.accessReviewInstanceDecisionItemResource",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String",
  "accessPackageId": "String",
  "accessPackageDisplayName": "String"
}
```


