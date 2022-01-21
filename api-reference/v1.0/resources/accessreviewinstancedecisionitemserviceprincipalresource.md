---
title: Tipo de recurso accessReviewInstanceDecisionItemServicePrincipalResource
description: Representa entidades de serviço cujo acesso a um recurso é representado por meio de um objeto accessReviewInstanceDecisionItem.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e71aacd0ac0876ed7ec9fc0fdc70b8f136831092
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162106"
---
# <a name="accessreviewinstancedecisionitemserviceprincipalresource-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItemServicePrincipalResource

Namespace: microsoft.graph

Representa entidades de serviço cujo acesso a um recurso é representado por meio de um [objeto accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md) **accessReviewInstanceDecisionItemServicePrincipalResource** é um tipo aberto que permite que outras propriedades sejam passadas.

Herda [de accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| appId | Cadeia de caracteres | O identificador global exclusivo do aplicativo ao qual o acesso foi concedido. |
| displayName | Cadeia de caracteres | Nome de exibição do recurso. Herdado [de accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).|
| id | Cadeia de caracteres | Identificador do recurso de item de decisão. Herdado [de accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |
| type | Cadeia de caracteres | Tipo de recurso. Tipo sempre será `ServicePrincipal` .  Herdado [de accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessreviewinstancedecisionitemserviceprincipalresource",
  "baseType": "microsoft.graph.accessReviewInstanceDecisionItemResource",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessreviewinstancedecisionitemserviceprincipalresource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String",
  "appId": "String"
}
```
