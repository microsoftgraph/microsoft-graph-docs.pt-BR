---
title: Tipo de recurso retentionLabel
description: Representa como os clientes podem gerenciar seus dados, seja por quanto tempo retê-los ou excluí-los.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 8e74f494b56c2a622510648953f1a021a32140c7
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447501"
---
# <a name="retentionlabel-resource-type"></a>Tipo de recurso retentionLabel

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa como os clientes podem gerenciar seus dados, incluindo se e por quanto tempo retê-los ou excluí-los.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar retentionLabels](../api/security-retentionlabel-list.md)|[coleção microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|Obtenha uma lista dos [objetos retentionLabel](../resources/security-retentionlabel.md) e suas propriedades.|
|[Criar retentionLabel](../api/security-retentionlabel-post.md)|[microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|Crie um novo [objeto retentionLabel](../resources/security-retentionlabel.md) .|
|[Obter retentionLabel](../api/security-retentionlabel-get.md)|[microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|Leia as propriedades e as relações de um [objeto retentionLabel](../resources/security-retentionlabel.md) .|
|[Atualizar retentionLabel](../api/security-retentionlabel-update.md)|[microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|Atualize as propriedades de um [objeto retentionLabel](../resources/security-retentionlabel.md) .|
|[Excluir retentionLabel](../api/security-retentionlabel-delete.md)|Nenhum|Exclua [um objeto retentionLabel](../resources/security-retentionlabel.md) .|
|[Listar retentionEventType](../api/security-retentioneventtype-list.md)|[coleção microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Obtenha os recursos retentionEventType da propriedade de navegação exapnd eventType.|
|[Adicionar retentionEventType](../api/security-retentioneventtype-post.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Adicione eventType adicionando a propriedade odata relevante ao criar um rótulo.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actionAfterRetentionPeriod|microsoft.graph.security.actionAfterRetentionPeriod| Especifica a ação a ser tomada em um documento com esse rótulo aplicado durante o período de retenção. Os valores possíveis são: `none`, `delete`, `startDispositionReview`, `unknownFutureValue`.|
|behaviorDuringRetentionPeriod|microsoft.graph.security.behaviorDuringRetentionPeriod|Especifica como o comportamento de um documento com esse rótulo deve ser durante o período de retenção. Os valores possíveis são: `doNotRetain`, `retain`, `retainAsRecord`, `retainAsRegulatoryRecord`, `unknownFutureValue`.|
|createdBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|Representa o usuário que criou o retentionLabel.|
|createdDateTime|DateTimeOffset|Representa a data e a hora em que o retentionLabel é criado.|
|descriptionForAdmins|Cadeia de caracteres|Fornece informações de rótulo para o administrador. Opcional.|
|descriptionForUsers|String|Fornece as informações de rótulo para o usuário. Opcional.|
|displayName|Cadeia de caracteres|Cadeia de caracteres exclusiva que define um nome de rótulo.|
|dispositionReviewStages|[coleção microsoft.graph.security.dispositionReviewStage](../resources/security-dispositionreviewstage.md)|Examine os estágios durante os quais os revisores são notificados para determinar se um documento deve ser excluído ou retido.|
|id|String|ID exclusiva do retentionLabel. [entidade](/graph/api/resources/entity).|
|isInUse|Booliano|Especifica se o rótulo está sendo usado no momento.|
|lastModifiedBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|O usuário que modificou o retentionLabel pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A data mais recente em que o retentionLabel foi modificado.|
|retentionDuration|[microsoft.graph.security.retentionDuration](../resources/security-retentionduration.md)|Especifica o número de dias para reter o conteúdo.|
|retentionTrigger|microsoft.graph.security.retentionTrigger|Especifica se a duração da retenção é calculada a partir da data de criação do conteúdo, da data rotulada ou da data da última modificação. Os valores possíveis são: `dateLabeled`, `dateCreated`, `dateModified`, `dateOfEvent`, `unknownFutureValue`.|
|defaultRecordBehavior|microsoft.graph.security.defaultRecordBehavior|Especifica o estado bloqueado ou desbloqueado de um rótulo de registro quando ele é criado. Os valores possíveis são: `startLocked`, `startUnlocked`, `unknownFutureValue`.|
|labelToBeApplied|Cadeia de caracteres|Especifica o rótulo de substituição a ser aplicado automaticamente após o término do período de retenção do rótulo atual. |


## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|dispositionReviewStages|[coleção microsoft.graph.security.dispositionReviewStage](../resources/security-dispositionreviewstage.md)|Quando a ação no final da retenção é escolhida como 'dispositionReview', dispositionReviewStages especifica um conjunto sequencial de estágios com pelo menos um revisor em cada estágio.|
|eventType|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Representa o tipo associado a um evento de retenção..|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.retentionLabel",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.retentionLabel",
  "id": "String (identifier)",
  "displayName": "String",
  "behaviorDuringRetentionPeriod": "String",
  "actionAfterRetentionPeriod": "String",
  "retentionTrigger": "String",
  "retentionDuration": {
    "@odata.type": "microsoft.graph.security.retentionDuration"
  },
  "isInUse": "Boolean",
  "descriptionForAdmins": "String",
  "descriptionForUsers": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "labelToBeApplied": "String",
  "defaultRecordBehavior": "String"
}
```
