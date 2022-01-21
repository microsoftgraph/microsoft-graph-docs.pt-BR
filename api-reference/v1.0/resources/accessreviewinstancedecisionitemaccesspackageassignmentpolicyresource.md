---
title: Tipo de recurso accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource
description: Representa uma política de atribuição de pacote de acesso para a qual o acesso é representado por meio de um objeto accessReviewInstanceDecisionItem.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3dfb5c9a42e9b807b802ff1e1ef24b2533388db4
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162111"
---
# <a name="accessreviewinstancedecisionitemaccesspackageassignmentpolicyresource-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource

Namespace: microsoft.graph

Representa uma política de atribuição de pacote de acesso para a qual o acesso é representado por meio de um [objeto accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md) **accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource** é um tipo aberto que permite que outras propriedades sejam passadas.

Herda [de accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|accessPackageDisplayName|Cadeia de caracteres| Nome de exibição do pacote de acesso ao qual o acesso foi concedido. |
|accessPackageId|Cadeia de caracteres| Identificador do pacote de acesso ao qual o acesso foi concedido. |
| displayName | Cadeia de caracteres | Nome de exibição do pacote de acesso. Herdado [de accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).|
| id | Cadeia de caracteres | Identificador do recurso de item de decisão. Herdado [de accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |
| type | Cadeia de caracteres | Tipo de recurso. Tipo sempre será `AccessPackageAssignmentPolicy` .  Herdado [de accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |



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


